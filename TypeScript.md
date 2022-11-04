# TypeScript cheatsheet

[React with TypeScript](https://www.freecodecamp.org/news/typescript-for-react-developers/#resources)
- Start reading in the useReducer Hook

## Types

* string
* number
* boolean
* any
* undefined
* null
* array
	* number[]
	* ArrayNumber

## Express

* package.json
	* "tsc" : "tsc"
* Execute `npm run tsc -- --init`
* Create the index.ts
* Execute `npm run tsc`
* Create script in "package.json" `"start" : "node ./build/index.js"`
* Install `ts-node-dev -D` and add the dev script


# Interfaces or Types

-   If you write object-oriented code, use interfaces. If you write functional code, use type aliases.
-   Use interfaces for public API libraries and types for components, state, JSX, etc.

# Enums

```javascript
const enum PATHS {
	HOME = "/home",
	MOVIE = "/movie/:id"
}

const STATUSCODE = {
	OK = 200,
	ERROR = 404
}
```


# DOM

```javascript
const form = document.querySelector("form") // HTMLFormElement | null

form.addEventListener((e: Event) => {
	console.log(e)
})

// Error, posibilly null
```

3 ways to fix this:

```javascript
const form = document.querySelector("form")! // You know this isn't null
```


```javascript
const form = document.querySelector("form")

form?.addEventListener((e: Event) => {
	console.log(e)
})

// If form isn't null, execute the addEventListener
```

Better for my opinion: 

```javascript
const form = document.querySelector("form") as HTMLFormElement // You know this is a HTMLFormElement and not null

form.addEventListener((e: Event) => {
	console.log(e)
})
```