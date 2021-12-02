# Ghost Static Website

## How to run locally

- Start WSL
- Run Ghost in docker using the content folder from this repository
  `docker run -d --name some-ghost -p 2368:2368 -v ${PWD}/content:/var/lib/ghost/content ghost:alpine`

## Login to the Ghost admin app

- `http://localhost:2368/ghost`

## Add posts or edit the layout etc

- Use the Ghost admin app

## View the website

- `http://localhost:2368`

## Deploy the website to Github Pages

- Just push to the main branch and GitHub workflow will run up the Ghost instance, crawl the site to generate a static website, and then push the static site to Github Pages.
