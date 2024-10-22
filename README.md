# Destack Demo Next.js Website

Welcome to the **Destack Demo Next.js Website**! This project demonstrates how to integrate [Destack](https://github.com/LiveDuo/destack) into a Next.js application, providing a user-friendly website builder dashboard. Users can easily switch themes, drag and drop sections, and manage their content seamlessly.

## Features

- **Website Builder Dashboard**: Users can switch between multiple themes and utilize drag-and-drop functionality to add sections such as FAQs, reviews, navigation, footers, forms, and more.
- **Multiple Pages**: Users can access the dashboard on two different pages: `/` and `/destack-demo`.
- **Custom Route Creation**: Easily create new routes to access the dashboard.

## Getting Started

Follow these instructions to set up the project on your local machine.

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (version 14 or higher)
- [npm](https://www.npmjs.com/get-npm) (comes with Node.js)

### Clone the Repository

1. Open your terminal.
2. Run the following command to clone the repository:

   ```bash
   git clone https://github.com/meet-bhimani/destack-demo-nextjs-pages-router.git
   ```

3. Navigate to the project directory:

   ```bash
   cd destack-demo-nextjs-pages-router
   ```

### Install Dependencies

To install the required dependencies, run:

```bash
 npm install
```

### Running the Development Server

To start the development server, execute:

```bash
 npm run dev
```

Once the server is running, open your browser and navigate to http://localhost:3000. You will see the website builder dashboard.

### Using the Website Builder

- On the dashboard, you can switch between different themes.
- Drag and drop various sections (like FAQ, reviews, navigation, footer, form, etc.) to customize your page.

### Accessing Different Pages

You can access the website builder dashboard on the following pages:

- **Homepage**: [http://localhost:3000/](http://localhost:3000/)
- **Demo Page**: [http://localhost:3000/destack-demo](http://localhost:3000/destack-demo)

### Building the application for development:

1. Run the following command to generate optimized production build

   ```javascript
   npm run build
   ```

2. To run the built application on port 3000, use:

   ```javascript
   npm start
   ```

### Creating New Routes

If you want to create a new route to access the dashboard, follow these steps:

1. Create a new file inside the `src/pages` directory. The filename should match the desired route name (e.g., for `/new-route`, create `new-route.tsx`).

2. Paste the following content into the new file:

   ```javascript
   export { getStaticProps } from "destack/build/server";
   export { ContentProvider as default } from "destack";
   ```

3. After creating the new file, build the application by running:

   ```javascript
   npm run build
   ```

4. To run the built application on port 3000, use:

   ```javascript
   npm start
   ```

### Conclusion

You now have a fully functional Next.js application integrated with Destack. This project provides an intuitive dashboard for managing your website content effortlessly.

## Contributing

If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Any improvements or suggestions are welcome!.

## Acknowledgments

- [Next.js](https://nextjs.org/) for the framework
- [Destack](https://github.com/LiveDuo/destack) for the content management system
