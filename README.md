# 956 Pixelflow Starter Site

A one-page business website template for the $100 Starter Site package. Everything lives in `index.html`, so it hosts free on GitHub Pages.

## Make a new client site

1. On GitHub, create a new repository named after the client (for example `garza-lawn`).
2. Upload `index.html` (and the client's photos) to it.
3. Open `index.html` and search for `EDIT`. Replace every sample value:
   - Business name, phone, city, headline and description
   - Brand colors in the `:root` block at the top (`--brand` is the main color)
   - Services and prices (copy or delete the `<article class="service">` blocks)
   - About paragraphs and the four quick facts
   - Reviews (real ones only, from the client's Google or Facebook page)
   - Hours, service area, Google Maps search address, Facebook link
4. Replace the "Client photo goes here" note with the client's photo:
   `<img src="photo.jpg" alt="Short description of the photo">`

## Put it online (GitHub Pages)

1. In the repository, open **Settings → Pages**.
2. Under **Source**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
3. After about a minute the site is live at `https://<your-github-name>.github.io/<repo-name>/`.

## Connect the client's domain

1. The client buys the domain in their own name.
2. In the repository, **Settings → Pages → Custom domain**: type the domain and save. GitHub adds a `CNAME` file.
3. At the domain company, add the DNS records GitHub shows on that page.
4. Once it checks green, tick **Enforce HTTPS**.

## Turn on the contact form

1. Create a free form at formspree.io using the client's email.
2. Copy the form address it gives you (looks like `https://formspree.io/f/abcdwxyz`).
3. In `index.html`, paste it into `data-endpoint="..."` on the `<form>` tag.

Until then, the form shows "Preview only: this form is not connected yet."

## Care Plan changes

Each change request = edit `index.html`, commit with a short note (for example "Update hours for December"), and the live site updates in about a minute. The commit history is your record of changes made each month.
