# Black Coffee :metal:

<p align="center">
  <img width="300" height="300" src="black-coffee-logo.png">
</p>

A coffee store mobile app built using Strapi, Koa, Apollo Server/GraphQL, Docker, Stripe and React Native.

## Background

This project was initially started for [Hacktober Fest 2019](https://hacktoberfest.digitalocean.com/), but it quickly grew into a playground of ideas I've had and new technologies I've been wanting to try out.

### Strapi

At the time I was really wanting to build something of some significance with Strapi since it had just went into beta. Since I started this I've been Strapi everyday at work so it turned out to be pretty good practice.

### Koa

I've been using Express forever and it's always gotten the job done. I try out new Node.js frameworks occasionally just see if they could be useful in future projects. So of course Koa has been on my list and I specifically grabbed for it in this project because I saw that Strapi used Koa under the hood. Honestly I don't really like it.

### Apollo

I've worked on some large GraphQL projects over the last couple years and they've used Apollo v1. I knew I was going to have to upgrade these projects to Apollo v2 at some point in the future so I figured I should start learning the differences.

### Docker

The entire project would be a pain to run withough `docker-compose`. Maybe in the future I'll actually deploy the containers on Kubernetes somewhere. I've never used a managed K8s service like Amazon EKS or GKE, so that could be a good reason to test it out.

### Stripe

I used Stripe on a pretty large project a while back and I just wanted to see if it was still as easy/nice/awesome as it was a couple years ago. And of course it is!

### React Native

I've used React Native a lot over the last couple years but I haven't used it with Stripe integration or GraphQL/Apollo Client. I also haven't used Expo on anything other than quick and dirty projects to test things out. For any significant mobile app with React Native I've always gone with the React Native CLI.

## Backend Architecture

![Black Coffee Backend Architecture](black-coffee-architecture.jpg)

## Running Everything

1. Clone the repo
2. `npm install` in each of the folders inside the `server` and `mobile` folders
3. Copy the `.env-example` and rename it to `.env`. The example should have all of the variables you will need and some already filled out.
4. In the `server` folder run `docker-compose up`.
5. The mobile app uses Expo to manage React Native so you will need to folow [these steps](https://docs.expo.io/get-started/installation/) to get it installed
6. In the `mobile` folder run `expo start`
