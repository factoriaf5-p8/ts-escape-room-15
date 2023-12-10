# Typescript Labs

## Lab 15: Combining Types to Create New Types

file: `/src/15-intersection.problem.ts`

Continuing with `User` and `Post`, we now have a `getDefaultUserAndPosts` function that has an `unknown` return type:

```ts
export const getDefaultUserAndPosts = (): unknown => {
  return {
    id: "1",
    firstName: "Matt",
    lastName: "Pocock",
    posts: [
      {
        id: "1",
        title: "How I eat so much cheese",
        body: "It's pretty edam difficult",
      },
    ],
  };
};
```

Challenge
Your challenge is to update the return type for the function so that it is both User and { posts: Post[] }.