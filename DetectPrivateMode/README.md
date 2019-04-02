# Detect Private Mode
This help function will detect Browser's Mode (Private or not) and return True (is private mode) or flase (is public mode)

## Implement Method
It checked different browsers if they still enable cookie, file system (depents on different browser's private method).

## Usage in Project
I used it when my project used localStorage to store user preferences. It will have differnece prefermance when browser is in private mode. So I used this support function to detect and remind user change the browser mode if they want fully service with preference settings.
It can be used in any cases if project needs to check different browser modes (e.g. if the project uses localStorage, sessionStorage, Cookie, file systems, etc.)

## Test case
```JavaScript
isPrivateMode().then((inPrivate) => {
    console.log(`is in private mode: ${inPrivate}`);
})
```