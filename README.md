# magaldi.dev

A simple website hosted on GitHub Pages with a custom domain.

## Setup Instructions

1. Push this repository to GitHub
2. Go to your repository settings on GitHub
3. Navigate to Pages section
4. Select the branch you want to deploy (usually `main`)
5. The site will be available at `https://yourusername.github.io/repository-name`
6. The `CNAME` file will automatically configure the custom domain `magaldi.dev`

## Custom Domain Configuration

1. In your DNS provider (where you manage magaldi.dev), add:

   - Type: `A` records pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - OR Type: `CNAME` record pointing to `yourusername.github.io`

2. Wait for DNS propagation (can take up to 48 hours)

3. In GitHub repository settings > Pages, verify that the custom domain appears

## Local Development

Simply open `index.html` in a web browser or use a local server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js http-server
npx http-server
```

Then visit `http://localhost:8000`
