# Identity

## [Intro to Identity](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-2.1&tabs=visual-studio)

>ASP.NET Core Identity is a membership system that adds login functionality to ASP.NET Core apps. Users can create an account with the login information stored in Identity or they can use an external login provider. Supported external login providers include Facebook, Google, Microsoft Account, and Twitter.
>
>Identity can be configured using a SQL Server database to store user names, passwords, and profile data. Alternatively, another persistent store can be used, for example, Azure Table Storage.

## [Identity Demystified](https://digitalmccullough.com/posts/aspnetcore-auth-system-demystified.html)

- > `Claim` represents a single fact about the user. It could be the user's first name, last name, age, employer, birth date, or anything else that is true about the user. A single claim will contain only a single piece of information. A claim representing something about a user John Smith could be his first name: John. A second claim would be his last name: Smith.

- `ClaimsIdentity` contains multiple `claims` to identify a user :
    > An Identity represents a form of identification or, in other words, a single way of proving who you are. In real life this could be a driver's license. In ASP.Net Core, it is a ClaimsIdentity. This class represents a single form of digital identification.

- `ClaimsPrincipal`: Principal that can contain multiple instances of `ClaimsIdentity`
    > A Principal represents the actual user. It can contain one or more instances of ClaimsIdentity, just like in life a person may have a driver's license, concealed-carry permit, social security card, and a passport. Each of the identities is used for a different purpose and may contain a unique set of claims, but they all identify the same user in some form or another.

- Verbs
  - Authenticate
    - Gets the user’s information if any exists (e.g. decoding the user’s cookie, if one exists)
- Challenge
  - Requests authentication by the user (e.g. showing a login page)
  
- SignIn
  - Persists the user’s information somewhere (e.g. writes a cookies)

- SignOut
  - Removes the user’s persisted information (e.g. deletes the cookies)

- Forbid
  - Denies access to a resource for unauthenticated users or authenticated but unauthorized users (e.g. displaying a “not authorized” page)
