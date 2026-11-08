# kriworden20.github.io
Personal website for Kristen Worden


# Preview Website Locally

https://willhoffer.com/2022-09-03/previewing-your-webpage-locally/

^ I followed the steps above, downloaded ruby 4.0.9 using chruby. I had to troubleshoot and have Gemini give me a new Gemfile for the Jekyll serve to work with this ruby version.

## 🚀 Local Development

Follow these steps to spin up the Jekyll preview environment locally on macOS.

### 1. Environment Verification
Ensure your terminal session is using the correct Ruby environment and that you are navigating directly to the source folder containing the dependencies:

```bash
# Verify active Ruby environment
ruby -v

# Navigate to the docs directory where the Gemfile resides
cd kriworden20.gitub.io/docs
```

### 2. Update / Install Dependencies
Run this whenever you pull updates down from the repository, alter the `Gemfile`, or setup a new machine to ensure your locked gem instances stay in sync:

```bash
# Clean up any conflicting lock files and download definitions
rm -f Gemfile.lock
bundle install
```

### 3. Launch the Server
Fire up the local Jekyll engine to compile your assets and serve the codebase:

```bash
bundle exec jekyll serve
```

### 4. View the Site
Once the build completes successfully, open your browser of choice and navigate to either:
👉 **[http://127.0.0.1:4000/](http://127.0.0.1:4000/)**
👉 **[http://localhost:4000/](http://localhost:4000/)**

> 💡 **Tip:** The server runs with **live reloading** active. Any saved updates to your layouts, assets, or markdown content will automatically trigger an incremental build and instantly push the changes to your browser view.

