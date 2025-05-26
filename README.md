# personal-website
Personal website of Jeremy W. Hopwood

To build, 
curl -X POST "https://api.cloudflare.com/client/v4/pages/webhooks/deploy_hooks/bcc3af90-e818-41a6-aa47-b12ee9ee7f2f"

Windows instructions:
Install Ruby: https://rubyinstaller.org
Enable Ruby in PowerShell (or Perl): ridk enable
Setup (in website source directory): bundle
Build and server locally: bundle exec jekyll serve