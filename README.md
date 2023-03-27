# Bard Utils

[![AI Friendly](https://img.shields.io/badge/AI-Friendly-pink?style=for-the-badge)](https://github.com/mefengl/made-by-ai)
[![AI Assisted Maybe](https://img.shields.io/badge/AI%20Assisted-Maybe-yellow?style=for-the-badge)](https://github.com/mefengl/made-by-ai)
[![Commit Messages by AI](https://img.shields.io/badge/Commit%20Messages%20by-AI-green?style=for-the-badge)](https://github.com/mefengl/made-by-ai)

## Notice

this repo will soon be put into `chat-kit`, you can find more about it in [chatgpt-playground](https://github.com/mefengl/chatgpt-playground)

## Description

getSubmitButton, getTextarea, getRegenerateButton, getNewChatButton...

## Usage

just copy and paste the code below

```js
function getInputArea() {
  return document.querySelector(".input-area");
};
```

```js
function getSubmitButton() {
  return document.querySelector('button[aria-label="Send message"]');
};
```

```js
function getTextarea() {
  const inputArea = getInputArea();
  return inputArea.querySelector('textarea');
};
```

```js
function getRegenerateButton() {
  return document.querySelector('button[aria-label="Retry"]');
};
```

```js
function getNewChatButton() {
  const navButtons = document.querySelector('mat-nav-list').children;
  return Array.from(navButtons).find(b => b.textContent.trim().toLowerCase().includes('reset chat'));
};
```

```js
function getLastResponse() {
  const responseElements = document.querySelectorAll('.model-response-text');
  const lastResponse = responseElements[responseElements.length - 1];
  return lastResponse;
};
```

```js
function getLastResponseText() {
  const lastResponse = getLastResponse();
  return lastResponse.textContent;
};
```

## Contributing

Contributions, issues and feature requests are welcome!

## License

This project is licensed under the terms of the [MIT license](/LICENSE).
