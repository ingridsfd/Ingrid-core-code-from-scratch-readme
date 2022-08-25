### API stablishment:
/* EXERCISE 9
Intro:

    PowerUsers idea was bad. Once those users got
    extended permissions, they started bullying others
    and we lost a lot of great users.
    As a response we spent all the remaining money
    on the marketing and got even more users.
    We need to start preparing to move everything to a
    real database. For now we just do some mocks.

    The server API format was decided to be the following:

    In case of success: { status: 'success', data: RESPONSE_DATA }
    In case of error: { status: 'error', error: ERROR_MESSAGE }

    The API engineer started creating types for this API and
    quickly figured out that the amount of types needed to be
    created is too big.

Exercise:

    Remove UsersApiResponse and AdminsApiResponse types
    and use generic type ApiResponse in order to specify API
    response formats for each of the functions.
*/
```JavaScript
export type ApiResponse<T> =
      | { status: 'success'; data: T; }
      | { status: 'error'; error: string; };

export function requestAdmins(callback: (response: ApiResponse<Admin[]>) => void) {
    callback({
        status: 'success',
        data: admins
    });
}

export function requestUsers(callback: (response: ApiResponse<User[]>) => void) {
    callback({
        status: 'success',
        data: users
    });
}

export function requestCurrentServerTime(callback: (response: ApiResponse<number>) => void) {
    callback({
        status: 'success',
        data: Date.now()
    });
}

export function requestCoffeeMachineQueueLength(callback: (response: ApiResponse<number>) => void) {
    callback({
        status: 'error',
        error: 'Numeric value has exceeded Number.MAX_SAFE_INTEGER.'
    });
}
```
### PROMISE BEHAVIOR
/* EXERCISE 10 

Intro:

    We have asynchronous functions now, advanced technology.
    This makes us a tech startup officially now.
    But one of the consultants spoiled our dreams about
    inevitable future IT leadership.
    He said that callback-based asynchronicity is not
    popular anymore and everyone should use Promises.
    He promised that if we switch to Promises, this would
    bring promising results.

Exercise:

    We don't want to reimplement all the data-requesting
    functions. Let's decorate the old callback-based
    functions with the new Promise-compatible result.
    The final function should return a Promise which
    would resolve with the final data directly
    (i.e. users or admins) or would reject with an error
    (or type Error).

    The function should be named promisify.

Higher difficulty bonus exercise:

    Create a function promisifyAll which accepts an object
    with functions and returns a new object where each of
    the function is promisified.

    Rewrite api creation accordingly:

        const api = promisifyAll(oldApi);

*/
