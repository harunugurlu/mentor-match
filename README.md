This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

### Clone the Repository

1. Open your terminal or command prompt.
2. Navigate to the directory where you want to clone the repository.
3. Run the following command to clone the repository:

```bash
git clone <repository-url>
```

Replace `<repository-url>` with the actual URL of the repository.

4. Navigate to the cloned repository directory:

```bash
cd <repository-name>
```

Replace `<repository-name>` with the name of your repository.

5. Install the project dependencies:

```bash
npm install
```

**Note:** Make sure you are in the root of your project directory before running the above command.

### Create a New Branch

After cloning the repository, it's a good practice to create a new branch for your feature work. Here's how you can do it:

1. Navigate to the cloned repository directory.
2. Run the following command to create a new branch:

```bash
git checkout -b <branch-name>
```

Replace `<branch-name>` with the name of your new branch.

Remember, it's a good practice to name the branch something that describes the feature you're working on.

### Setup DB

1. Either run it locally or create a cloud DB.

#### Local

1. `docker run --name mongodb -d -p 27017:27017 mongodb/mongodb-community-server:latest`

### Copy .env.example to .env.local

1. `cp .env.example .env.local`
1. Modify the `MONGO_URI` string to your DB connection _(the default string is for local DB connection)_

Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
