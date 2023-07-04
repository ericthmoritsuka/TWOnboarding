## Can use the build_site.sh script to build Liferay Learn locally

I was using some build_site.sh script when I was fixing links with Russ. I created these aliases to help me:

\`\`\`
alias lbuild="cd ~/dev/projects/liferay-learn/site && ./build_site.sh"
alias lcleanbuild="cd ~/dev/projects/liferay-learn/site && rm -r venv && rm -r build && ./build_site.sh"
alias lsync="cd ~/dev/projects/liferay-learn && g co master && g stash && g pull upstream master && git push origin master"
\`\`\`

I was using lbuild to build the site from the liferay-learn local repository, lcleanbuild to perform a clean build where I removed some of the files before building the site and lsync just to sync the repo.

Last time I used it was in March or April. So, I am not sure if something has changed since.