# @shipsecure/eslint-plugin-next

## Overview

`@shipsecure/eslint-plugin-next` is a custom ESLint plugin designed to enhance the security of Next.js applications by identifying potentially insecure patterns in code. This plugin offers a set of rules specifically tailored to prevent common security pitfalls in Next.js, encouraging best practices and securing your app's frontend and backend code.

## Features

- Rules for Secure Code: Detects usage of unsecure URLs, inline scripts, eval, and other potential security vulnerabilities.
- Recommended Configurations: Provides a recommended set of rules for immediate security improvements.
- Easy to Integrate: Seamlessly integrates with any Next.js project with simple installation and configuration.

## Installation

```bash
npm install @shipsecure/eslint-plugin-next --save-dev
```

## Usage

### Basic Configuration

To start using the plugin in your Next.js project, add `@shipsecure/eslint-plugin-next` to your ESLint configuration file (e.g., `.eslintrc.js`):

```javascript
module.exports = {
  extends: [
    "eslint:recommended",
    "plugin:@shipsecure/next/recommended", // Use the recommended configuration
  ],
  plugins: ["@shipsecure/next"],
};
```

### Custom Configuration

If you want to enable or disable specific rules, add them to the rules section in your ESLint configuration:

```javascript
module.exports = {
  plugins: ["@shipsecure/next"],
  rules: {
    "@shipsecure/next/no-open-redirects": "error",
    // Add other rules here
  },
};
```

## Contributing

Contributions are welcome! If you'd like to add new rules, suggest enhancements, or report issues, please open a pull request or issue on our [GitHub repository](https://github.com/shipsecure-labs/eslint-plugin-next).

### Steps to Contribute

<ol>
<li>Fork the repository.</li>
<li>Create a new branch for your feature (git checkout -b feature-name).</li>
<li>Make your changes and add tests.</li>
<li>Run tests to ensure everything works (npm test).</li>
<li>Push your branch and submit a pull request.</li>
</ol>

## License

This project is licensed under the MIT License - see the LICENSE file for details.