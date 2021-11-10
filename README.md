
# YouTube-Videos-As-Posts
YouTube Videos As Posts

## YouTube Videos As Posts Features:
1. Free Hosting using GitHub Pages and open-source code base in GitHub.
2. It can update all the videos, title, and description available inside the channel into the posts in jekyll site structure everyday automatically using the GitHub Actions feature.
2. No need to manually do any step after posting any new video in YouTube, it will be updated in website on next day.

## How to Reuse this Action Template which creates a personal website for the YouTube videos in my channel hosted in Github Pages using Jekyll and Github Actions for free!

1. Copy this Github Action below:

```
   - name: YouTube-Videos-As-Posts
     uses: SSanjeevi/YouTubeVideosAsPosts@Release1.0.0
     with:
     GoogleApiKey: ${{ secrets.GoogleApiKey }}
     channelName: 'channel_Name'
     
   - name: Commit and push update
     run: |-
     git config --global user.email "youremailid@gmail.com"
     git config --global user.name "yourUserName"
     git add -A
     git commit -m "Updated Youtube Video posts from GitHub Actions"
     git push

``` 

2. Use any Jekyll Theme for the repo
3. Keep the posts folder empty - this Action will create all the videos as posts in the repository
4. You are ready with website with Videos embedded in Github Pages


## Samples created by this tool:

## Demo 1:
https://chemistry.lkgforit.com/

## Demo 2:
https://tv.lkgforit.com/

## Demo 3
https://tnpsc.lkgforit.com

## Detailed Article:
[Step by Step Tutorial](https://lkgforit.com/personal-youtube-channel-videos-website-hosted-in-github-pages-for-free-which-populates-content-by-itself)


Reference:

https://github.com/dsebastien/youtubeChannelVideosFinder

https://github.com/nathancy/jekyll-embed-video
