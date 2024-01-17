# The Postroom

## Features

Here are some of the features that The Postroom offers:

- Post directly to social media from within the platform
- Manage your team within the application
- Schedule notifications for social media posts

## Tech Stack

The Postroom is built on top of the following technologies:

- A [GitHub](https://github.com/) account
- [Next.js](https://nextjs.org/) - framework
- [TypeScript](https://www.typescriptlang.org/) - language
- [Tailwind](https://tailwindcss.com/) - CSS
- [Redis](https://redis.com/) - redis
- [Tinybird](https://tinybird.com/) - analytics (coming soon)
- [MySQL](https://mysql.com/) - database
- [NextAuth.js](https://next-auth.js.org/) - auth
- [BullMQ](https://https://docs.bullmq.io/) - queue worker
- [Stripe](https://stripe.com/) - payments (coming soon)
- [Mailing](https://www.mailing.run/) - emails
- [Laravel Forge](https://forge.laravel.com/) - deployments (frontend)

### Development

#### Step 1: Local setup

First, clone the [The Postroom repo](https://github.com/Bond-and-Coyne/ThePostRoom) GitHub repository.

```bash
git clone git@github.com:Bond-and-Coyne/ThePostRoom.git
```

Run the following command to install the dependencies:

```bash
cd next && yarn
```

Convert the `.env.template` file to `.env`. 

<Info>If you require access, please contact [Craig](mailto:craig@bondandcoyne.co.uk) or [Dan](mailto:daniel@bondandcoyne.co.uk)</Info>

Setup self signed certificates within the folder to run the local version on SSL

<Info>We use mkcert install via [Brew](https://formulae.brew.sh/formula/mkcert)</Info>

<Info>This app runs on a '.app' subdomain, so you may also need to update your hosts file to include `app.localhost 127.0.0.1`</Info>

```bash
mkcert app.localhost
```

Finally we can run the dev server which will automatically proxy ssl from `port 3000`
```bash
yarn dev
```