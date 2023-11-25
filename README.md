# next-rails-scaffold

The gem [next_rails_scaffold](https://github.com/raphox/next-rails) uses this repository to generate the page routing system to consume the RESTful API generated by the command `bin/rails generate scaffold Post title:string body:text`.

To get more information about the page routing system and the static export for Next.js, access https://nextjs.org/docs/pages/building-your-application/deploying/static-exports.
To learn more about the Rails scaffold generator, access https://guides.rubyonrails.org/command_line.html#bin-rails-generate.

## Templates

```
_templates/scaffold/
└── javascript
    ├── [id]
    |   ├── edit.ejs.t
    |   └── show.ejs.t
    ├── components
    |   ├── resource.ejs.t
    |   └── resource_form.ejs.t
    ├── home.js
    ├── index.js
    ├── list.ejs.t
    ├── new.ejs.t
    └── services.ejs.t
├── typescript (TODO)
└── shadcn-ui (TODO)
```

## Frontend tech stack:

- **Next.js (https://nextjs.org)** - _The React Framework for the Web_
  - Elevate our frontend development by leveraging Next.js, a powerful React Framework tailored for the web. Join us in creating and managing a dynamic and responsive web application with enhanced performance and developer-friendly features.
- **Axios (https://axios-http.com)** - _Promise based HTTP client for the browser and node.js_
  - Empower our application with Axios, a versatile and promise-based HTTP client. Contribute to setting up a global request configuration, defining custom headers, and handling exceptions and success responses. Ensure smooth communication between the browser and node.js.
- **React Query (https://tanstack.com/query/latest)** - _Powerful asynchronous state management for TS/JS, React, Solid, Vue, and Svelte_
  - Transform the way we handle asynchronous state management using React Query. Collaborate with us to seamlessly load and update data through RESTful requests. Bring your expertise in TypeScript/JavaScript, React, Solid, Vue, or Svelte to enhance our application's state management capabilities.
- **React Hook Form (https://react-hook-form.com)** - _Performant, flexible, and extensible forms with easy-to-use validation_
  - Contribute to building high-performance, flexible, and extensible forms with React Hook Form. Your role involves defining and implementing robust form validations, ensuring an effortless and error-free user experience. Join us in creating dynamic and user-friendly forms.
- **Zod (https://zod.dev)** - _TypeScript-first schema validation with static type inference_
  - Enhance our application's integrity with Zod, a TypeScript-first schema validation tool. Work with us to define and enforce validation rules, leveraging static type inference for a more secure and type-safe codebase. Ensure data consistency and reliability.
- **Hygen (https://www.hygen.io)** - _The scalable code generator that saves you time_
  - Optimize our development workflow with Hygen, a scalable code generator designed to save time. Play a crucial role in defining and utilizing templates for our code generation process. Improve code consistency and reduce repetitive tasks by incorporating Hygen into our project.

## Using

```
npm install
npx hygen generator scaffold post title:string body:text
```

### Result

Generated files strutucture:

```
src
├── components
|   ├── Post.js
|   └── PostForm.js
├── pages
|   └── posts
|       ├── [id]
|       |   ├── edit.js
|       |   └── index.js
|       ├── index.js
|       └── new.js
└── services.js
```

Sample app https://github.com/raphox/next-rails-app.
