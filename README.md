# Harry's Personal Website

Author: Harry He

> To visit the production version of the site, you can check out [the website](https://heisharry.vercel.app/).

## Project Description

First off, a cool image with the branding colors because nobody really clicks on the [contact](https://heisharry.vercel.app/contact) page.
<p align="center">
   <img width="auto" src="/static/ContactHeader.webp" />
</p>

The website is Harry's personal website containing information about Harry's projects, skills, and professional history.

### Development Tools Used
- **SvelteKit**: Web framework used to develop the site
- **Open Props**: Modern CSS library used to handle design consistency
- **PostCSS (Just In Time) Props**: Extension used to optimize Open Props variables
- **FormSubmit**: Backend API used to route email messages

### Asset Generation

As with many Web Development projects, many assets had to be generated to be put onto the website. Here are some of the tools used to create the images that you see on the website.
- **Photoshop**: Image editor used to capture Harry and design images with special effects
- **Google Drawings**: Virtual board used to create thumbnail images of projects
- **Figma**: Design tool used to generate logos and set up SVG animations

## Dependencies
Site was developed with [Node](https://nodejs.org/) >= v18, optional [pnpm](https://pnpm.io/) for managing node packages, [Svelte](https://svelte.dev/) version 4.0.0, and [Open Props](https://open-props.style/) version 1.5.10.

## Adapting This Project
To develop a site with the same stack, you can use Harry's SvelteKit-Template on the [postcss-open-props branch](https://github.com/he-is-harry/SvelteKit-Template/tree/postcss-open-props) to use Svelte, Open Props, and PostCSS (Just In Time) Props.

To simply copy in the template run the following command.

```
git clone -b postcss-open-props --single-branch https://github.com/he-is-harry/SvelteKit-Template.git
```