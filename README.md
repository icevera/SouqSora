# SouqSora

SouqSora is a simple, developer-friendly, open-source e-commerce application designed with beginners in mind. Built with modern tools and a straightforward architecture, it empowers developers to create, customize, and deploy e-commerce platforms effortlessly.

## Why "SouqSora"?
The name **SouqSora** reflects the essence of the project:

- **"Souq"** (سوق): An Arabic word meaning "market," symbolizing the application's purpose as a commerce platform.
- **"Sora"** (空): A Japanese word meaning "sky," representing openness, freedom, and limitless possibilities.

Together, "SouqSora" conveys the vision of a flexible, open-source e-commerce solution that bridges cultures and innovation.

## Features
1. **Simplicity**: Built to be easy for beginners to understand and modify.
2. **Framework**: Developed with [SvelteKit](https://kit.svelte.dev/), ensuring fast and reactive user experiences.
3. **API**: The backend API is also powered by SvelteKit, streamlining development.
4. **Database**: Uses [Prisma](https://www.prisma.io/) as the ORM and [PostgreSQL](https://www.postgresql.org/) as the database.
5. **Deployment**:
   - Can be hosted on serverless platforms (e.g., Vercel, Netlify).
   - Includes a pre-configured Docker file and [Kamal 2.0](https://kamal.io/) file for containerized deployments.
6. **Testing**:
   - [Cypress](https://www.cypress.io/) is integrated for end-to-end testing.
   - [Storybook](https://storybook.js.org/) is set up for UI component development and testing.
7. **TypeScript**: Written in TypeScript with non-strict mode enabled, balancing type safety with flexibility.
8. **Styling**: Uses [Tailwind CSS](https://tailwindcss.com/) for rapid UI design and customization.

## Installation
### Prerequisites
- Node.js (v16 or later)
- PostgreSQL
- Docker (optional for containerized deployment)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/souqsora.git
   cd souqsora
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up the environment:
   - Create a `.env` file in the root directory.
   - Add your database connection string and other required environment variables.

4. Run database migrations:
   ```bash
   npx prisma migrate dev
   ```
5. Start the development server:
   ```bash
   npm run dev
   ```

## Deployment
- **Serverless Hosting**: Use platforms like Vercel or Netlify for seamless serverless deployment.
- **Docker**:
  - Build and run the container:
    ```bash
    docker build -t souqsora .
    docker run -p 3000:3000 souqsora
    ```
- **Kamal 2.0**: Leverage the provided `kamal.yml` file for advanced container orchestration.

## Testing
- Run end-to-end tests with Cypress:
  ```bash
  npm run test:e2e
  ```
- View and test UI components with Storybook:
  ```bash
  npm run storybook
  ```

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests. Check the `CONTRIBUTING.md` file for guidelines.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
