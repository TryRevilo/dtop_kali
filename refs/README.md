





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">



  <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/frameworks-3b630179b3ba661bed136319970519c14eae34456b7cf575d1126c208cd61d0e.css" media="all" rel="stylesheet" />
  <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-adef29b21c28620124e601ee69f4b175d336f5fba00d9b75685d91beb2c6373d.css" media="all" rel="stylesheet" />
  
  
  <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/site-85e343141d26757cd1c83e11a4fdf25acae930572a5436fe5b5f0e521468930f.css" media="all" rel="stylesheet" />
  

  <meta name="viewport" content="width=device-width">
  
  <title>youtube-dl/README.md at master · rg3/youtube-dl · GitHub</title>
  <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    
    <meta content="https://avatars2.githubusercontent.com/u/53487?v=3&amp;s=400" property="og:image" /><meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="rg3/youtube-dl" property="og:title" /><meta content="https://github.com/rg3/youtube-dl" property="og:url" /><meta content="youtube-dl - Command-line program to download videos from YouTube.com and other video sites" property="og:description" />

  <link rel="assets" href="https://assets-cdn.github.com/">
  
  <meta name="pjax-timeout" content="1000">
  
  <meta name="request-id" content="C6FA:4749:22E5007:33CD940:593B18A3" data-pjax-transient>
  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

  <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
    <meta name="google-analytics" content="UA-3769691-2">

<meta content="collector.githubapp.com" name="octolytics-host" /><meta content="github" name="octolytics-app-id" /><meta content="https://collector.githubapp.com/github-external/browser_event" name="octolytics-event-url" /><meta content="C6FA:4749:22E5007:33CD940:593B18A3" name="octolytics-dimension-request_id" /><meta content="iad" name="octolytics-dimension-region_edge" /><meta content="iad" name="octolytics-dimension-region_render" />
<meta content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" name="analytics-location" />




  <meta class="js-ga-set" name="dimension1" content="Logged Out">


  

      <meta name="hostname" content="github.com">
  <meta name="user-login" content="">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="OWE2MTc1ZDQwYTllMTY3ZGEwZTZlMWFhZGUzMTg2ZDA5MjdmMzA4MjViNDMyNzVlZWVmYmEyMDQ3ZTAyMTY1Nnx7InJlbW90ZV9hZGRyZXNzIjoiMTk3LjIzNy4xOTQuMTY1IiwicmVxdWVzdF9pZCI6IkM2RkE6NDc0OToyMkU1MDA3OjMzQ0Q5NDA6NTkzQjE4QTMiLCJ0aW1lc3RhbXAiOjE0OTcwNDUxNTcsImhvc3QiOiJnaXRodWIuY29tIn0=">


  <meta name="html-safe-nonce" content="845c3cd7d09c892a43c4ee033067fa1424095345">

  <meta http-equiv="x-pjax-version" content="379b97800ad43e21019100841c41525b">
  

    
  <meta name="description" content="youtube-dl - Command-line program to download videos from YouTube.com and other video sites">
  <meta name="go-import" content="github.com/rg3/youtube-dl git https://github.com/rg3/youtube-dl.git">

  <meta content="53487" name="octolytics-dimension-user_id" /><meta content="rg3" name="octolytics-dimension-user_login" /><meta content="1039520" name="octolytics-dimension-repository_id" /><meta content="rg3/youtube-dl" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="1039520" name="octolytics-dimension-repository_network_root_id" /><meta content="rg3/youtube-dl" name="octolytics-dimension-repository_network_root_nwo" /><meta content="false" name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" />
  <link href="https://github.com/rg3/youtube-dl/commits/master.atom" rel="alternate" title="Recent Commits to youtube-dl:master" type="application/atom+xml">


    <link rel="canonical" href="https://github.com/rg3/youtube-dl/blob/master/README.md" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

<meta name="theme-color" content="#1e2327">



  </head>

  <body class="logged-out env-production page-blob">
    



  <div class="position-relative js-header-wrapper ">
    <a href="#start-of-content" tabindex="1" class="px-2 py-4 show-on-focus js-skip-to-content">Skip to content</a>
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>

    
    
    



          <header class="site-header js-details-container Details" role="banner">
  <div class="site-nav-container">
    <a class="header-logo-invertocat" href="https://github.com/" aria-label="Homepage" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="32" version="1.1" viewBox="0 0 16 16" width="32"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
    </a>

    <button class="btn-link float-right site-header-toggle js-details-target" type="button" aria-label="Toggle navigation">
      <svg aria-hidden="true" class="octicon octicon-three-bars" height="24" version="1.1" viewBox="0 0 12 16" width="18"><path fill-rule="evenodd" d="M11.41 9H.59C0 9 0 8.59 0 8c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zm0-4H.59C0 5 0 4.59 0 4c0-.59 0-1 .59-1H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1h.01zM.59 11H11.4c.59 0 .59.41.59 1 0 .59 0 1-.59 1H.59C0 13 0 12.59 0 12c0-.59 0-1 .59-1z"/></svg>
    </button>

    <div class="site-header-menu">
      <nav class="site-header-nav">
        <a href="/features" class="js-selected-navigation-item nav-item" data-ga-click="Header, click, Nav menu - item:features" data-selected-links="/features /features">
          Features
</a>        <a href="/business" class="js-selected-navigation-item nav-item" data-ga-click="Header, click, Nav menu - item:business" data-selected-links="/business /business/security /business/customers /business">
          Business
</a>        <a href="/explore" class="js-selected-navigation-item nav-item" data-ga-click="Header, click, Nav menu - item:explore" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship /showcases /explore">
          Explore
</a>            <a href="/marketplace" class="js-selected-navigation-item nav-item" data-ga-click="Header, click, Nav menu - item:marketplace" data-selected-links=" /marketplace">
              Marketplace
</a>        <a href="/pricing" class="js-selected-navigation-item nav-item" data-ga-click="Header, click, Nav menu - item:pricing" data-selected-links="/pricing /pricing/developer /pricing/team /pricing/business-hosted /pricing/business-enterprise /pricing">
          Pricing
</a>      </nav>

      <div class="site-header-actions">
          <div class="header-search scoped-search site-scoped-search js-site-search" role="search">
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="/rg3/youtube-dl/search" class="js-site-search-form" data-scoped-search-url="/rg3/youtube-dl/search" data-unscoped-search-url="/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <label class="form-control header-search-wrapper js-chromeless-input-container">
        <a href="/rg3/youtube-dl/blob/master/README.md" class="header-search-scope no-underline">This repository</a>
      <input type="text"
        class="form-control header-search-input js-site-search-focus js-site-search-field is-clearable"
        data-hotkey="s"
        name="q"
        value=""
        placeholder="Search"
        aria-label="Search this repository"
        data-unscoped-placeholder="Search GitHub"
        data-scoped-placeholder="Search"
        autocapitalize="off">
        <input type="hidden" class="js-site-search-type-field" name="type" >
    </label>
</form></div>


          <a class="text-bold site-header-link" href="/login?return_to=%2Frg3%2Fyoutube-dl%2Fblob%2Fmaster%2FREADME.md" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
            <span class="text-gray">or</span>
            <a class="text-bold site-header-link" href="/join?source=header-repo" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
      </div>
    </div>
  </div>
</header>


  </div>

  <div id="start-of-content" class="show-on-focus"></div>

    <div id="js-flash-container">
</div>



  <div role="main">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode">
    <div id="js-repo-pjax-container" data-pjax-container>
      

      



    <div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav">
      <div class="container repohead-details-container">

        <ul class="pagehead-actions">
  <li>
      <a href="/login?return_to=%2Frg3%2Fyoutube-dl"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <svg aria-hidden="true" class="octicon octicon-eye" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
    Watch
  </a>
  <a class="social-count" href="/rg3/youtube-dl/watchers"
     aria-label="1079 users are watching this repository">
    1,079
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2Frg3%2Fyoutube-dl"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <svg aria-hidden="true" class="octicon octicon-star" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74z"/></svg>
    Star
  </a>

    <a class="social-count js-social-count" href="/rg3/youtube-dl/stargazers"
      aria-label="26525 users starred this repository">
      26,525
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2Frg3%2Fyoutube-dl"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <svg aria-hidden="true" class="octicon octicon-repo-forked" height="16" version="1.1" viewBox="0 0 10 16" width="10"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
        Fork
      </a>

    <a href="/rg3/youtube-dl/network" class="social-count"
       aria-label="5026 users forked this repository">
      5,026
    </a>
  </li>
</ul>

        <h1 class="public ">
  <svg aria-hidden="true" class="octicon octicon-repo" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a href="/rg3" class="url fn" rel="author">rg3</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a href="/rg3/youtube-dl" data-pjax="#js-repo-pjax-container">youtube-dl</a></strong>

</h1>

      </div>
      <div class="container">
        
<nav class="reponav js-repo-nav js-sidenav-container-pjax"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/rg3/youtube-dl" class="js-selected-navigation-item selected reponav-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /rg3/youtube-dl" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-code" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a href="/rg3/youtube-dl/issues" class="js-selected-navigation-item reponav-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /rg3/youtube-dl/issues" itemprop="url">
        <svg aria-hidden="true" class="octicon octicon-issue-opened" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="Counter">1,488</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a href="/rg3/youtube-dl/pulls" class="js-selected-navigation-item reponav-item" data-hotkey="g p" data-selected-links="repo_pulls /rg3/youtube-dl/pulls" itemprop="url">
      <svg aria-hidden="true" class="octicon octicon-git-pull-request" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">203</span>
      <meta itemprop="position" content="3">
</a>  </span>

    <a href="/rg3/youtube-dl/projects" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /rg3/youtube-dl/projects">
      <svg aria-hidden="true" class="octicon octicon-project" height="16" version="1.1" viewBox="0 0 15 16" width="15"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      Projects
      <span class="Counter" >0</span>
</a>


    <div class="reponav-dropdown js-menu-container">
      <button type="button" class="btn-link reponav-item reponav-dropdown js-menu-target " data-no-toggle aria-expanded="false" aria-haspopup="true">
        Insights
        <svg aria-hidden="true" class="octicon octicon-triangle-down v-align-middle text-gray" height="11" version="1.1" viewBox="0 0 12 16" width="8"><path fill-rule="evenodd" d="M0 5l6 6 6-6z"/></svg>
      </button>
      <div class="dropdown-menu-content js-menu-content">
        <div class="dropdown-menu dropdown-menu-sw">
          <a class="dropdown-item" href="/rg3/youtube-dl/pulse" data-skip-pjax>
            <svg aria-hidden="true" class="octicon octicon-pulse" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M11.5 8L8.8 5.4 6.6 8.5 5.5 1.6 2.38 8H0v2h3.6l.9-1.8.9 5.4L9 8.5l1.6 1.5H14V8z"/></svg>
            Pulse
          </a>
          <a class="dropdown-item" href="/rg3/youtube-dl/graphs" data-skip-pjax>
            <svg aria-hidden="true" class="octicon octicon-graph" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
            Graphs
          </a>
        </div>
      </div>
    </div>
</nav>

      </div>
    </div>

<div class="container new-discussion-timeline experiment-repo-nav">
  <div class="repository-content">

    
        
        



    
  <a href="/rg3/youtube-dl/blob/1afd0b0da70b6ed709c610aff98786d71511a629/README.md" class="d-none js-permalink-shortcut" data-hotkey="y">Permalink</a>

  <!-- blob contrib key: blob_contributors:v21:599a2cfceeeaa849fb01b823e580f9d9 -->

  <div class="file-navigation js-zeroclipboard-container">
    
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class=" btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
      <i>Branch:</i>
      <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax>

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg aria-label="Close" class="octicon octicon-x js-menu-close" height="16" role="img" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/rg3/youtube-dl/blob/download-server/README.md"
               data-name="download-server"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                download-server
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/rg3/youtube-dl/blob/gh-pages/README.md"
               data-name="gh-pages"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                gh-pages
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/rg3/youtube-dl/blob/master/README.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/rg3/youtube-dl/blob/rtmp_test/README.md"
               data-name="rtmp_test"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                rtmp_test
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
               href="/rg3/youtube-dl/blob/totalwebcasting/README.md"
               data-name="totalwebcasting"
               data-skip-pjax="true"
               rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                totalwebcasting
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.06.05/README.md"
              data-name="2017.06.05"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.06.05">
                2017.06.05
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.29/README.md"
              data-name="2017.05.29"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.29">
                2017.05.29
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.26/README.md"
              data-name="2017.05.26"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.26">
                2017.05.26
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.23/README.md"
              data-name="2017.05.23"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.23">
                2017.05.23
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.18.1/README.md"
              data-name="2017.05.18.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.18.1">
                2017.05.18.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.18/README.md"
              data-name="2017.05.18"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.18">
                2017.05.18
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.14/README.md"
              data-name="2017.05.14"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.14">
                2017.05.14
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.09/README.md"
              data-name="2017.05.09"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.09">
                2017.05.09
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.07/README.md"
              data-name="2017.05.07"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.07">
                2017.05.07
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.05.01/README.md"
              data-name="2017.05.01"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.05.01">
                2017.05.01
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.28/README.md"
              data-name="2017.04.28"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.28">
                2017.04.28
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.26/README.md"
              data-name="2017.04.26"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.26">
                2017.04.26
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.17/README.md"
              data-name="2017.04.17"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.17">
                2017.04.17
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.16/README.md"
              data-name="2017.04.16"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.16">
                2017.04.16
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.15/README.md"
              data-name="2017.04.15"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.15">
                2017.04.15
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.14/README.md"
              data-name="2017.04.14"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.14">
                2017.04.14
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.11/README.md"
              data-name="2017.04.11"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.11">
                2017.04.11
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.09/README.md"
              data-name="2017.04.09"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.09">
                2017.04.09
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.03/README.md"
              data-name="2017.04.03"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.03">
                2017.04.03
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.04.02/README.md"
              data-name="2017.04.02"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.04.02">
                2017.04.02
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.26/README.md"
              data-name="2017.03.26"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.26">
                2017.03.26
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.24/README.md"
              data-name="2017.03.24"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.24">
                2017.03.24
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.22/README.md"
              data-name="2017.03.22"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.22">
                2017.03.22
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.20/README.md"
              data-name="2017.03.20"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.20">
                2017.03.20
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.16/README.md"
              data-name="2017.03.16"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.16">
                2017.03.16
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.15/README.md"
              data-name="2017.03.15"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.15">
                2017.03.15
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.10/README.md"
              data-name="2017.03.10"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.10">
                2017.03.10
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.07/README.md"
              data-name="2017.03.07"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.07">
                2017.03.07
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.06/README.md"
              data-name="2017.03.06"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.06">
                2017.03.06
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.05/README.md"
              data-name="2017.03.05"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.05">
                2017.03.05
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.03.02/README.md"
              data-name="2017.03.02"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.03.02">
                2017.03.02
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.28/README.md"
              data-name="2017.02.28"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.28">
                2017.02.28
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.27/README.md"
              data-name="2017.02.27"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.27">
                2017.02.27
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.24.1/README.md"
              data-name="2017.02.24.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.24.1">
                2017.02.24.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.24/README.md"
              data-name="2017.02.24"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.24">
                2017.02.24
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.22/README.md"
              data-name="2017.02.22"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.22">
                2017.02.22
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.21/README.md"
              data-name="2017.02.21"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.21">
                2017.02.21
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.17/README.md"
              data-name="2017.02.17"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.17">
                2017.02.17
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.16/README.md"
              data-name="2017.02.16"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.16">
                2017.02.16
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.14/README.md"
              data-name="2017.02.14"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.14">
                2017.02.14
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.11/README.md"
              data-name="2017.02.11"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.11">
                2017.02.11
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.10/README.md"
              data-name="2017.02.10"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.10">
                2017.02.10
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.07/README.md"
              data-name="2017.02.07"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.07">
                2017.02.07
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.04.1/README.md"
              data-name="2017.02.04.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.04.1">
                2017.02.04.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.04/README.md"
              data-name="2017.02.04"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.04">
                2017.02.04
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.02.01/README.md"
              data-name="2017.02.01"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.02.01">
                2017.02.01
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.31/README.md"
              data-name="2017.01.31"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.31">
                2017.01.31
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.29/README.md"
              data-name="2017.01.29"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.29">
                2017.01.29
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.28/README.md"
              data-name="2017.01.28"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.28">
                2017.01.28
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.25/README.md"
              data-name="2017.01.25"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.25">
                2017.01.25
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.24/README.md"
              data-name="2017.01.24"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.24">
                2017.01.24
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.22/README.md"
              data-name="2017.01.22"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.22">
                2017.01.22
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.18/README.md"
              data-name="2017.01.18"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.18">
                2017.01.18
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.16/README.md"
              data-name="2017.01.16"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.16">
                2017.01.16
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.14/README.md"
              data-name="2017.01.14"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.14">
                2017.01.14
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.10/README.md"
              data-name="2017.01.10"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.10">
                2017.01.10
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.08/README.md"
              data-name="2017.01.08"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.08">
                2017.01.08
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.05/README.md"
              data-name="2017.01.05"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.05">
                2017.01.05
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2017.01.02/README.md"
              data-name="2017.01.02"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2017.01.02">
                2017.01.02
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.31/README.md"
              data-name="2016.12.31"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.31">
                2016.12.31
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.22/README.md"
              data-name="2016.12.22"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.22">
                2016.12.22
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.20/README.md"
              data-name="2016.12.20"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.20">
                2016.12.20
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.18/README.md"
              data-name="2016.12.18"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.18">
                2016.12.18
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.15/README.md"
              data-name="2016.12.15"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.15">
                2016.12.15
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.12/README.md"
              data-name="2016.12.12"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.12">
                2016.12.12
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.09/README.md"
              data-name="2016.12.09"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.09">
                2016.12.09
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.12.01/README.md"
              data-name="2016.12.01"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.12.01">
                2016.12.01
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.27/README.md"
              data-name="2016.11.27"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.27">
                2016.11.27
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.22/README.md"
              data-name="2016.11.22"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.22">
                2016.11.22
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.18/README.md"
              data-name="2016.11.18"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.18">
                2016.11.18
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.14.1/README.md"
              data-name="2016.11.14.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.14.1">
                2016.11.14.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.14/README.md"
              data-name="2016.11.14"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.14">
                2016.11.14
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.08.1/README.md"
              data-name="2016.11.08.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.08.1">
                2016.11.08.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.08/README.md"
              data-name="2016.11.08"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.08">
                2016.11.08
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.04/README.md"
              data-name="2016.11.04"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.04">
                2016.11.04
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.11.02/README.md"
              data-name="2016.11.02"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.11.02">
                2016.11.02
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.31/README.md"
              data-name="2016.10.31"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.31">
                2016.10.31
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.30/README.md"
              data-name="2016.10.30"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.30">
                2016.10.30
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.26/README.md"
              data-name="2016.10.26"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.26">
                2016.10.26
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.25/README.md"
              data-name="2016.10.25"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.25">
                2016.10.25
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.21.1/README.md"
              data-name="2016.10.21.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.21.1">
                2016.10.21.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.21/README.md"
              data-name="2016.10.21"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.21">
                2016.10.21
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.19/README.md"
              data-name="2016.10.19"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.19">
                2016.10.19
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.16/README.md"
              data-name="2016.10.16"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.16">
                2016.10.16
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.12/README.md"
              data-name="2016.10.12"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.12">
                2016.10.12
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.07/README.md"
              data-name="2016.10.07"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.07">
                2016.10.07
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.10.02/README.md"
              data-name="2016.10.02"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.10.02">
                2016.10.02
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.27/README.md"
              data-name="2016.09.27"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.27">
                2016.09.27
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.24/README.md"
              data-name="2016.09.24"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.24">
                2016.09.24
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.19/README.md"
              data-name="2016.09.19"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.19">
                2016.09.19
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.18/README.md"
              data-name="2016.09.18"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.18">
                2016.09.18
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.15/README.md"
              data-name="2016.09.15"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.15">
                2016.09.15
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.11.1/README.md"
              data-name="2016.09.11.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.11.1">
                2016.09.11.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.11/README.md"
              data-name="2016.09.11"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.11">
                2016.09.11
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.08/README.md"
              data-name="2016.09.08"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.08">
                2016.09.08
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.04.1/README.md"
              data-name="2016.09.04.1"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.04.1">
                2016.09.04.1
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.04/README.md"
              data-name="2016.09.04"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.04">
                2016.09.04
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.09.03/README.md"
              data-name="2016.09.03"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.09.03">
                2016.09.03
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.08.31/README.md"
              data-name="2016.08.31"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.08.31">
                2016.08.31
              </span>
            </a>
            <a class="select-menu-item js-navigation-item js-navigation-open "
              href="/rg3/youtube-dl/tree/2016.08.28/README.md"
              data-name="2016.08.28"
              data-skip-pjax="true"
              rel="nofollow">
              <svg aria-hidden="true" class="octicon octicon-check select-menu-item-icon" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5z"/></svg>
              <span class="select-menu-item-text css-truncate-target" title="2016.08.28">
                2016.08.28
              </span>
            </a>
        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

    <div class="BtnGroup float-right">
      <a href="/rg3/youtube-dl/find/master"
            class="js-pjax-capture-input btn btn-sm BtnGroup-item"
            data-pjax
            data-hotkey="t">
        Find file
      </a>
      <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm BtnGroup-item tooltipped tooltipped-s" data-copied-hint="Copied!" type="button">Copy path</button>
    </div>
    <div class="breadcrumb js-zeroclipboard-target">
      <span class="repo-root js-repo-root"><span class="js-path-segment"><a href="/rg3/youtube-dl"><span>youtube-dl</span></a></span></span><span class="separator">/</span><strong class="final-path">README.md</strong>
    </div>
  </div>


  
  <div class="commit-tease">
      <span class="float-right">
        <a class="commit-tease-sha" href="/rg3/youtube-dl/commit/76e6378358a618a20051e9f9fd38e43af3169683" data-pjax>
          76e6378
        </a>
        <relative-time datetime="2017-06-08T15:02:42Z">Jun 8, 2017</relative-time>
      </span>
      <div>
        <img alt="@dstftw" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/1908898?v=3&amp;s=40" width="20" />
        <a href="/dstftw" class="user-mention" rel="contributor">dstftw</a>
          <a href="/rg3/youtube-dl/commit/76e6378358a618a20051e9f9fd38e43af3169683" class="message" data-pjax="true" title="[README.md] Improve man page formatting">[README.md] Improve man page formatting</a>
      </div>

    <div class="commit-tease-contributors">
      <button type="button" class="btn-link muted-link contributors-toggle" data-facebox="#blob_contributors_box">
        <strong>49</strong>
         contributors
      </button>
          <a class="avatar-link tooltipped tooltipped-s" aria-label="phihag" href="/rg3/youtube-dl/commits/master/README.md?author=phihag"><img alt="@phihag" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/779568?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="dstftw" href="/rg3/youtube-dl/commits/master/README.md?author=dstftw"><img alt="@dstftw" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/1908898?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="jaimeMF" href="/rg3/youtube-dl/commits/master/README.md?author=jaimeMF"><img alt="@jaimeMF" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/1239727?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="FiloSottile" href="/rg3/youtube-dl/commits/master/README.md?author=FiloSottile"><img alt="@FiloSottile" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/1225294?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="yan12125" href="/rg3/youtube-dl/commits/master/README.md?author=yan12125"><img alt="@yan12125" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/1937689?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="habi" href="/rg3/youtube-dl/commits/master/README.md?author=habi"><img alt="@habi" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/1651235?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="aurium" href="/rg3/youtube-dl/commits/master/README.md?author=aurium"><img alt="@aurium" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/30254?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="jwilk" href="/rg3/youtube-dl/commits/master/README.md?author=jwilk"><img alt="@jwilk" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/141546?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="iemejia" href="/rg3/youtube-dl/commits/master/README.md?author=iemejia"><img alt="@iemejia" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/79476?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="michael-k" href="/rg3/youtube-dl/commits/master/README.md?author=michael-k"><img alt="@michael-k" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/152008?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="WassimAttar" href="/rg3/youtube-dl/commits/master/README.md?author=WassimAttar"><img alt="@WassimAttar" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/5887870?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="TomGijselinck" href="/rg3/youtube-dl/commits/master/README.md?author=TomGijselinck"><img alt="@TomGijselinck" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/3659344?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="raunaqrox" href="/rg3/youtube-dl/commits/master/README.md?author=raunaqrox"><img alt="@raunaqrox" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/2609361?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="remitamine" href="/rg3/youtube-dl/commits/master/README.md?author=remitamine"><img alt="@remitamine" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/10879694?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="rbrito" href="/rg3/youtube-dl/commits/master/README.md?author=rbrito"><img alt="@rbrito" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/212145?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="pulpe" href="/rg3/youtube-dl/commits/master/README.md?author=pulpe"><img alt="@pulpe" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/763046?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="psjay" href="/rg3/youtube-dl/commits/master/README.md?author=psjay"><img alt="@psjay" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/856285?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="terminalmage" href="/rg3/youtube-dl/commits/master/README.md?author=terminalmage"><img alt="@terminalmage" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/328598?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="rpunkfu" href="/rg3/youtube-dl/commits/master/README.md?author=rpunkfu"><img alt="@rpunkfu" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/7048281?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="Nikoli" href="/rg3/youtube-dl/commits/master/README.md?author=Nikoli"><img alt="@Nikoli" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/444492?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="nikai3d" href="/rg3/youtube-dl/commits/master/README.md?author=nikai3d"><img alt="@nikai3d" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/494755?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="Bassoon08" href="/rg3/youtube-dl/commits/master/README.md?author=Bassoon08"><img alt="@Bassoon08" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/1066522?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="mark7" href="/rg3/youtube-dl/commits/master/README.md?author=mark7"><img alt="@mark7" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/2308945?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="jeffcrouse" href="/rg3/youtube-dl/commits/master/README.md?author=jeffcrouse"><img alt="@jeffcrouse" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/15384?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="vitorgalvao" href="/rg3/youtube-dl/commits/master/README.md?author=vitorgalvao"><img alt="@vitorgalvao" class="avatar" height="20" src="https://avatars2.githubusercontent.com/u/1699443?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="hub2git" href="/rg3/youtube-dl/commits/master/README.md?author=hub2git"><img alt="@hub2git" class="avatar" height="20" src="https://avatars0.githubusercontent.com/u/7141051?v=3&amp;s=40" width="20" /> </a>

    <button type="button" data-facebox="#blob_contributors_box" class="btn-link others-text">and others</button>

    </div>

    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@phihag" height="24" src="https://avatars3.githubusercontent.com/u/779568?v=3&amp;s=48" width="24" />
            <a href="/phihag">phihag</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@dstftw" height="24" src="https://avatars1.githubusercontent.com/u/1908898?v=3&amp;s=48" width="24" />
            <a href="/dstftw">dstftw</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jaimeMF" height="24" src="https://avatars1.githubusercontent.com/u/1239727?v=3&amp;s=48" width="24" />
            <a href="/jaimeMF">jaimeMF</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@FiloSottile" height="24" src="https://avatars3.githubusercontent.com/u/1225294?v=3&amp;s=48" width="24" />
            <a href="/FiloSottile">FiloSottile</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@yan12125" height="24" src="https://avatars3.githubusercontent.com/u/1937689?v=3&amp;s=48" width="24" />
            <a href="/yan12125">yan12125</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@habi" height="24" src="https://avatars0.githubusercontent.com/u/1651235?v=3&amp;s=48" width="24" />
            <a href="/habi">habi</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@aurium" height="24" src="https://avatars0.githubusercontent.com/u/30254?v=3&amp;s=48" width="24" />
            <a href="/aurium">aurium</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jwilk" height="24" src="https://avatars1.githubusercontent.com/u/141546?v=3&amp;s=48" width="24" />
            <a href="/jwilk">jwilk</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@iemejia" height="24" src="https://avatars3.githubusercontent.com/u/79476?v=3&amp;s=48" width="24" />
            <a href="/iemejia">iemejia</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@michael-k" height="24" src="https://avatars0.githubusercontent.com/u/152008?v=3&amp;s=48" width="24" />
            <a href="/michael-k">michael-k</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@WassimAttar" height="24" src="https://avatars3.githubusercontent.com/u/5887870?v=3&amp;s=48" width="24" />
            <a href="/WassimAttar">WassimAttar</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@TomGijselinck" height="24" src="https://avatars0.githubusercontent.com/u/3659344?v=3&amp;s=48" width="24" />
            <a href="/TomGijselinck">TomGijselinck</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@raunaqrox" height="24" src="https://avatars1.githubusercontent.com/u/2609361?v=3&amp;s=48" width="24" />
            <a href="/raunaqrox">raunaqrox</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@remitamine" height="24" src="https://avatars3.githubusercontent.com/u/10879694?v=3&amp;s=48" width="24" />
            <a href="/remitamine">remitamine</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@rbrito" height="24" src="https://avatars3.githubusercontent.com/u/212145?v=3&amp;s=48" width="24" />
            <a href="/rbrito">rbrito</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@pulpe" height="24" src="https://avatars1.githubusercontent.com/u/763046?v=3&amp;s=48" width="24" />
            <a href="/pulpe">pulpe</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@psjay" height="24" src="https://avatars3.githubusercontent.com/u/856285?v=3&amp;s=48" width="24" />
            <a href="/psjay">psjay</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@terminalmage" height="24" src="https://avatars2.githubusercontent.com/u/328598?v=3&amp;s=48" width="24" />
            <a href="/terminalmage">terminalmage</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@rpunkfu" height="24" src="https://avatars2.githubusercontent.com/u/7048281?v=3&amp;s=48" width="24" />
            <a href="/rpunkfu">rpunkfu</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Nikoli" height="24" src="https://avatars3.githubusercontent.com/u/444492?v=3&amp;s=48" width="24" />
            <a href="/Nikoli">Nikoli</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@nikai3d" height="24" src="https://avatars2.githubusercontent.com/u/494755?v=3&amp;s=48" width="24" />
            <a href="/nikai3d">nikai3d</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Bassoon08" height="24" src="https://avatars3.githubusercontent.com/u/1066522?v=3&amp;s=48" width="24" />
            <a href="/Bassoon08">Bassoon08</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@mark7" height="24" src="https://avatars1.githubusercontent.com/u/2308945?v=3&amp;s=48" width="24" />
            <a href="/mark7">mark7</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jeffcrouse" height="24" src="https://avatars2.githubusercontent.com/u/15384?v=3&amp;s=48" width="24" />
            <a href="/jeffcrouse">jeffcrouse</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@vitorgalvao" height="24" src="https://avatars0.githubusercontent.com/u/1699443?v=3&amp;s=48" width="24" />
            <a href="/vitorgalvao">vitorgalvao</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@hub2git" height="24" src="https://avatars2.githubusercontent.com/u/7141051?v=3&amp;s=48" width="24" />
            <a href="/hub2git">hub2git</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Reventl0v" height="24" src="https://avatars2.githubusercontent.com/u/5124130?v=3&amp;s=48" width="24" />
            <a href="/Reventl0v">Reventl0v</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@glisignoli" height="24" src="https://avatars0.githubusercontent.com/u/336538?v=3&amp;s=48" width="24" />
            <a href="/glisignoli">glisignoli</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@ryandesign" height="24" src="https://avatars1.githubusercontent.com/u/429209?v=3&amp;s=48" width="24" />
            <a href="/ryandesign">ryandesign</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@JackDanger" height="24" src="https://avatars3.githubusercontent.com/u/2071?v=3&amp;s=48" width="24" />
            <a href="/JackDanger">JackDanger</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@jakeogh" height="24" src="https://avatars1.githubusercontent.com/u/53795?v=3&amp;s=48" width="24" />
            <a href="/jakeogh">jakeogh</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Eun" height="24" src="https://avatars2.githubusercontent.com/u/796084?v=3&amp;s=48" width="24" />
            <a href="/Eun">Eun</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Laneone" height="24" src="https://avatars2.githubusercontent.com/u/3431687?v=3&amp;s=48" width="24" />
            <a href="/Laneone">Laneone</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@drguildo" height="24" src="https://avatars2.githubusercontent.com/u/9282?v=3&amp;s=48" width="24" />
            <a href="/drguildo">drguildo</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@cyberjacob" height="24" src="https://avatars3.githubusercontent.com/u/161093?v=3&amp;s=48" width="24" />
            <a href="/cyberjacob">cyberjacob</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@reddraggone9" height="24" src="https://avatars3.githubusercontent.com/u/2711644?v=3&amp;s=48" width="24" />
            <a href="/reddraggone9">reddraggone9</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@CharlieTLe" height="24" src="https://avatars3.githubusercontent.com/u/3375195?v=3&amp;s=48" width="24" />
            <a href="/CharlieTLe">CharlieTLe</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@epitron" height="24" src="https://avatars2.githubusercontent.com/u/16409?v=3&amp;s=48" width="24" />
            <a href="/epitron">epitron</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Blue9" height="24" src="https://avatars2.githubusercontent.com/u/12224008?v=3&amp;s=48" width="24" />
            <a href="/Blue9">Blue9</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@barlik" height="24" src="https://avatars2.githubusercontent.com/u/10207442?v=3&amp;s=48" width="24" />
            <a href="/barlik">barlik</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@TRox1972" height="24" src="https://avatars1.githubusercontent.com/u/10253943?v=3&amp;s=48" width="24" />
            <a href="/TRox1972">TRox1972</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@bentley" height="24" src="https://avatars0.githubusercontent.com/u/126009?v=3&amp;s=48" width="24" />
            <a href="/bentley">bentley</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@alexvong1995" height="24" src="https://avatars3.githubusercontent.com/u/10696787?v=3&amp;s=48" width="24" />
            <a href="/alexvong1995">alexvong1995</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@josephfrazier" height="24" src="https://avatars0.githubusercontent.com/u/6473925?v=3&amp;s=48" width="24" />
            <a href="/josephfrazier">josephfrazier</a>
          </li>
      </ul>
    </div>
  </div>

  <div class="file">
    <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a href="/rg3/youtube-dl/raw/master/README.md" class="btn btn-sm BtnGroup-item" id="raw-url">Raw</a>
        <a href="/rg3/youtube-dl/blame/master/README.md" class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b">Blame</a>
      <a href="/rg3/youtube-dl/commits/master/README.md" class="btn btn-sm BtnGroup-item" rel="nofollow">History</a>
    </div>


        <button type="button" class="btn-octicon disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <svg aria-hidden="true" class="octicon octicon-pencil" height="16" version="1.1" viewBox="0 0 14 16" width="14"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
        </button>
        <button type="button" class="btn-octicon btn-octicon-danger disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <svg aria-hidden="true" class="octicon octicon-trashcan" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
        </button>
  </div>

  <div class="file-info">
      1286 lines (954 sloc)
      <span class="file-info-divider"></span>
    85.2 KB
  </div>
</div>

    
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><p>youtube-dl - download videos from youtube.com or other video platforms</p>
<ul>
<li><a href="#installation">INSTALLATION</a></li>
<li><a href="#description">DESCRIPTION</a></li>
<li><a href="#options">OPTIONS</a></li>
<li><a href="#configuration">CONFIGURATION</a></li>
<li><a href="#output-template">OUTPUT TEMPLATE</a></li>
<li><a href="#format-selection">FORMAT SELECTION</a></li>
<li><a href="#video-selection">VIDEO SELECTION</a></li>
<li><a href="#faq">FAQ</a></li>
<li><a href="#developer-instructions">DEVELOPER INSTRUCTIONS</a></li>
<li><a href="#embedding-youtube-dl">EMBEDDING YOUTUBE-DL</a></li>
<li><a href="#bugs">BUGS</a></li>
<li><a href="#copyright">COPYRIGHT</a></li>
</ul>
<h1><a id="user-content-installation" class="anchor" href="#installation" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>INSTALLATION</h1>
<p>To install it right away for all UNIX users (Linux, OS X, etc.), type:</p>
<pre><code>sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl
</code></pre>
<p>If you do not have curl, you can alternatively use a recent wget:</p>
<pre><code>sudo wget https://yt-dl.org/downloads/latest/youtube-dl -O /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl
</code></pre>
<p>Windows users can <a href="https://yt-dl.org/latest/youtube-dl.exe">download an .exe file</a> and place it in any location on their <a href="http://en.wikipedia.org/wiki/PATH_%28variable%29">PATH</a> except for <code>%SYSTEMROOT%\System32</code> (e.g. <strong>do not</strong> put in <code>C:\Windows\System32</code>).</p>
<p>You can also use pip:</p>
<pre><code>sudo -H pip install --upgrade youtube-dl
</code></pre>
<p>This command will update youtube-dl if you have already installed it. See the <a href="https://pypi.python.org/pypi/youtube_dl">pypi page</a> for more information.</p>
<p>OS X users can install youtube-dl with <a href="http://brew.sh/">Homebrew</a>:</p>
<pre><code>brew install youtube-dl
</code></pre>
<p>Or with <a href="https://www.macports.org/">MacPorts</a>:</p>
<pre><code>sudo port install youtube-dl
</code></pre>
<p>Alternatively, refer to the <a href="#developer-instructions">developer instructions</a> for how to check out and work with the git repository. For further options, including PGP signatures, see the <a href="https://rg3.github.io/youtube-dl/download.html">youtube-dl Download Page</a>.</p>
<h1><a id="user-content-description" class="anchor" href="#description" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>DESCRIPTION</h1>
<p><strong>youtube-dl</strong> is a command-line program to download videos from YouTube.com and a few more sites. It requires the Python interpreter, version 2.6, 2.7, or 3.2+, and it is not platform specific. It should work on your Unix box, on Windows or on Mac OS X. It is released to the public domain, which means you can modify it, redistribute it or use it however you like.</p>
<pre><code>youtube-dl [OPTIONS] URL [URL...]
</code></pre>
<h1><a id="user-content-options" class="anchor" href="#options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>OPTIONS</h1>
<pre><code>-h, --help                       Print this help text and exit
--version                        Print program version and exit
-U, --update                     Update this program to latest version. Make
                                 sure that you have sufficient permissions
                                 (run with sudo if needed)
-i, --ignore-errors              Continue on download errors, for example to
                                 skip unavailable videos in a playlist
--abort-on-error                 Abort downloading of further videos (in the
                                 playlist or the command line) if an error
                                 occurs
--dump-user-agent                Display the current browser identification
--list-extractors                List all supported extractors
--extractor-descriptions         Output descriptions of all supported
                                 extractors
--force-generic-extractor        Force extraction to use the generic
                                 extractor
--default-search PREFIX          Use this prefix for unqualified URLs. For
                                 example "gvsearch2:" downloads two videos
                                 from google videos for youtube-dl "large
                                 apple". Use the value "auto" to let
                                 youtube-dl guess ("auto_warning" to emit a
                                 warning when guessing). "error" just throws
                                 an error. The default value "fixup_error"
                                 repairs broken URLs, but emits an error if
                                 this is not possible instead of searching.
--ignore-config                  Do not read configuration files. When given
                                 in the global configuration file
                                 /etc/youtube-dl.conf: Do not read the user
                                 configuration in ~/.config/youtube-
                                 dl/config (%APPDATA%/youtube-dl/config.txt
                                 on Windows)
--config-location PATH           Location of the configuration file; either
                                 the path to the config or its containing
                                 directory.
--flat-playlist                  Do not extract the videos of a playlist,
                                 only list them.
--mark-watched                   Mark videos watched (YouTube only)
--no-mark-watched                Do not mark videos watched (YouTube only)
--no-color                       Do not emit color codes in output
</code></pre>
<h2><a id="user-content-network-options" class="anchor" href="#network-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Network Options:</h2>
<pre><code>--proxy URL                      Use the specified HTTP/HTTPS/SOCKS proxy.
                                 To enable experimental SOCKS proxy, specify
                                 a proper scheme. For example
                                 socks5://127.0.0.1:1080/. Pass in an empty
                                 string (--proxy "") for direct connection
--socket-timeout SECONDS         Time to wait before giving up, in seconds
--source-address IP              Client-side IP address to bind to
-4, --force-ipv4                 Make all connections via IPv4
-6, --force-ipv6                 Make all connections via IPv6
</code></pre>
<h2><a id="user-content-geo-restriction" class="anchor" href="#geo-restriction" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Geo Restriction:</h2>
<pre><code>--geo-verification-proxy URL     Use this proxy to verify the IP address for
                                 some geo-restricted sites. The default
                                 proxy specified by --proxy (or none, if the
                                 options is not present) is used for the
                                 actual downloading.
--geo-bypass                     Bypass geographic restriction via faking
                                 X-Forwarded-For HTTP header (experimental)
--no-geo-bypass                  Do not bypass geographic restriction via
                                 faking X-Forwarded-For HTTP header
                                 (experimental)
--geo-bypass-country CODE        Force bypass geographic restriction with
                                 explicitly provided two-letter ISO 3166-2
                                 country code (experimental)
</code></pre>
<h2><a id="user-content-video-selection" class="anchor" href="#video-selection" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Video Selection:</h2>
<pre><code>--playlist-start NUMBER          Playlist video to start at (default is 1)
--playlist-end NUMBER            Playlist video to end at (default is last)
--playlist-items ITEM_SPEC       Playlist video items to download. Specify
                                 indices of the videos in the playlist
                                 separated by commas like: "--playlist-items
                                 1,2,5,8" if you want to download videos
                                 indexed 1, 2, 5, 8 in the playlist. You can
                                 specify range: "--playlist-items
                                 1-3,7,10-13", it will download the videos
                                 at index 1, 2, 3, 7, 10, 11, 12 and 13.
--match-title REGEX              Download only matching titles (regex or
                                 caseless sub-string)
--reject-title REGEX             Skip download for matching titles (regex or
                                 caseless sub-string)
--max-downloads NUMBER           Abort after downloading NUMBER files
--min-filesize SIZE              Do not download any videos smaller than
                                 SIZE (e.g. 50k or 44.6m)
--max-filesize SIZE              Do not download any videos larger than SIZE
                                 (e.g. 50k or 44.6m)
--date DATE                      Download only videos uploaded in this date
--datebefore DATE                Download only videos uploaded on or before
                                 this date (i.e. inclusive)
--dateafter DATE                 Download only videos uploaded on or after
                                 this date (i.e. inclusive)
--min-views COUNT                Do not download any videos with less than
                                 COUNT views
--max-views COUNT                Do not download any videos with more than
                                 COUNT views
--match-filter FILTER            Generic video filter. Specify any key (see
                                 help for -o for a list of available keys)
                                 to match if the key is present, !key to
                                 check if the key is not present, key &gt;
                                 NUMBER (like "comment_count &gt; 12", also
                                 works with &gt;=, &lt;, &lt;=, !=, =) to compare
                                 against a number, key = 'LITERAL' (like
                                 "uploader = 'Mike Smith'", also works with
                                 !=) to match against a string literal and &amp;
                                 to require multiple matches. Values which
                                 are not known are excluded unless you put a
                                 question mark (?) after the operator. For
                                 example, to only match videos that have
                                 been liked more than 100 times and disliked
                                 less than 50 times (or the dislike
                                 functionality is not available at the given
                                 service), but who also have a description,
                                 use --match-filter "like_count &gt; 100 &amp;
                                 dislike_count &lt;? 50 &amp; description" .
--no-playlist                    Download only the video, if the URL refers
                                 to a video and a playlist.
--yes-playlist                   Download the playlist, if the URL refers to
                                 a video and a playlist.
--age-limit YEARS                Download only videos suitable for the given
                                 age
--download-archive FILE          Download only videos not listed in the
                                 archive file. Record the IDs of all
                                 downloaded videos in it.
--include-ads                    Download advertisements as well
                                 (experimental)
</code></pre>
<h2><a id="user-content-download-options" class="anchor" href="#download-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Download Options:</h2>
<pre><code>-r, --limit-rate RATE            Maximum download rate in bytes per second
                                 (e.g. 50K or 4.2M)
-R, --retries RETRIES            Number of retries (default is 10), or
                                 "infinite".
--fragment-retries RETRIES       Number of retries for a fragment (default
                                 is 10), or "infinite" (DASH, hlsnative and
                                 ISM)
--skip-unavailable-fragments     Skip unavailable fragments (DASH, hlsnative
                                 and ISM)
--abort-on-unavailable-fragment  Abort downloading when some fragment is not
                                 available
--keep-fragments                 Keep downloaded fragments on disk after
                                 downloading is finished; fragments are
                                 erased by default
--buffer-size SIZE               Size of download buffer (e.g. 1024 or 16K)
                                 (default is 1024)
--no-resize-buffer               Do not automatically adjust the buffer
                                 size. By default, the buffer size is
                                 automatically resized from an initial value
                                 of SIZE.
--playlist-reverse               Download playlist videos in reverse order
--playlist-random                Download playlist videos in random order
--xattr-set-filesize             Set file xattribute ytdl.filesize with
                                 expected file size (experimental)
--hls-prefer-native              Use the native HLS downloader instead of
                                 ffmpeg
--hls-prefer-ffmpeg              Use ffmpeg instead of the native HLS
                                 downloader
--hls-use-mpegts                 Use the mpegts container for HLS videos,
                                 allowing to play the video while
                                 downloading (some players may not be able
                                 to play it)
--external-downloader COMMAND    Use the specified external downloader.
                                 Currently supports
                                 aria2c,avconv,axel,curl,ffmpeg,httpie,wget
--external-downloader-args ARGS  Give these arguments to the external
                                 downloader
</code></pre>
<h2><a id="user-content-filesystem-options" class="anchor" href="#filesystem-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Filesystem Options:</h2>
<pre><code>-a, --batch-file FILE            File containing URLs to download ('-' for
                                 stdin)
--id                             Use only video ID in file name
-o, --output TEMPLATE            Output filename template, see the "OUTPUT
                                 TEMPLATE" for all the info
--autonumber-start NUMBER        Specify the start value for %(autonumber)s
                                 (default is 1)
--restrict-filenames             Restrict filenames to only ASCII
                                 characters, and avoid "&amp;" and spaces in
                                 filenames
-w, --no-overwrites              Do not overwrite files
-c, --continue                   Force resume of partially downloaded files.
                                 By default, youtube-dl will resume
                                 downloads if possible.
--no-continue                    Do not resume partially downloaded files
                                 (restart from beginning)
--no-part                        Do not use .part files - write directly
                                 into output file
--no-mtime                       Do not use the Last-modified header to set
                                 the file modification time
--write-description              Write video description to a .description
                                 file
--write-info-json                Write video metadata to a .info.json file
--write-annotations              Write video annotations to a
                                 .annotations.xml file
--load-info-json FILE            JSON file containing the video information
                                 (created with the "--write-info-json"
                                 option)
--cookies FILE                   File to read cookies from and dump cookie
                                 jar in
--cache-dir DIR                  Location in the filesystem where youtube-dl
                                 can store some downloaded information
                                 permanently. By default
                                 $XDG_CACHE_HOME/youtube-dl or
                                 ~/.cache/youtube-dl . At the moment, only
                                 YouTube player files (for videos with
                                 obfuscated signatures) are cached, but that
                                 may change.
--no-cache-dir                   Disable filesystem caching
--rm-cache-dir                   Delete all filesystem cache files
</code></pre>
<h2><a id="user-content-thumbnail-images" class="anchor" href="#thumbnail-images" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Thumbnail images:</h2>
<pre><code>--write-thumbnail                Write thumbnail image to disk
--write-all-thumbnails           Write all thumbnail image formats to disk
--list-thumbnails                Simulate and list all available thumbnail
                                 formats
</code></pre>
<h2><a id="user-content-verbosity--simulation-options" class="anchor" href="#verbosity--simulation-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Verbosity / Simulation Options:</h2>
<pre><code>-q, --quiet                      Activate quiet mode
--no-warnings                    Ignore warnings
-s, --simulate                   Do not download the video and do not write
                                 anything to disk
--skip-download                  Do not download the video
-g, --get-url                    Simulate, quiet but print URL
-e, --get-title                  Simulate, quiet but print title
--get-id                         Simulate, quiet but print id
--get-thumbnail                  Simulate, quiet but print thumbnail URL
--get-description                Simulate, quiet but print video description
--get-duration                   Simulate, quiet but print video length
--get-filename                   Simulate, quiet but print output filename
--get-format                     Simulate, quiet but print output format
-j, --dump-json                  Simulate, quiet but print JSON information.
                                 See --output for a description of available
                                 keys.
-J, --dump-single-json           Simulate, quiet but print JSON information
                                 for each command-line argument. If the URL
                                 refers to a playlist, dump the whole
                                 playlist information in a single line.
--print-json                     Be quiet and print the video information as
                                 JSON (video is still being downloaded).
--newline                        Output progress bar as new lines
--no-progress                    Do not print progress bar
--console-title                  Display progress in console titlebar
-v, --verbose                    Print various debugging information
--dump-pages                     Print downloaded pages encoded using base64
                                 to debug problems (very verbose)
--write-pages                    Write downloaded intermediary pages to
                                 files in the current directory to debug
                                 problems
--print-traffic                  Display sent and read HTTP traffic
-C, --call-home                  Contact the youtube-dl server for debugging
--no-call-home                   Do NOT contact the youtube-dl server for
                                 debugging
</code></pre>
<h2><a id="user-content-workarounds" class="anchor" href="#workarounds" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Workarounds:</h2>
<pre><code>--encoding ENCODING              Force the specified encoding (experimental)
--no-check-certificate           Suppress HTTPS certificate validation
--prefer-insecure                Use an unencrypted connection to retrieve
                                 information about the video. (Currently
                                 supported only for YouTube)
--user-agent UA                  Specify a custom user agent
--referer URL                    Specify a custom referer, use if the video
                                 access is restricted to one domain
--add-header FIELD:VALUE         Specify a custom HTTP header and its value,
                                 separated by a colon ':'. You can use this
                                 option multiple times
--bidi-workaround                Work around terminals that lack
                                 bidirectional text support. Requires bidiv
                                 or fribidi executable in PATH
--sleep-interval SECONDS         Number of seconds to sleep before each
                                 download when used alone or a lower bound
                                 of a range for randomized sleep before each
                                 download (minimum possible number of
                                 seconds to sleep) when used along with
                                 --max-sleep-interval.
--max-sleep-interval SECONDS     Upper bound of a range for randomized sleep
                                 before each download (maximum possible
                                 number of seconds to sleep). Must only be
                                 used along with --min-sleep-interval.
</code></pre>
<h2><a id="user-content-video-format-options" class="anchor" href="#video-format-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Video Format Options:</h2>
<pre><code>-f, --format FORMAT              Video format code, see the "FORMAT
                                 SELECTION" for all the info
--all-formats                    Download all available video formats
--prefer-free-formats            Prefer free video formats unless a specific
                                 one is requested
-F, --list-formats               List all available formats of requested
                                 videos
--youtube-skip-dash-manifest     Do not download the DASH manifests and
                                 related data on YouTube videos
--merge-output-format FORMAT     If a merge is required (e.g.
                                 bestvideo+bestaudio), output to given
                                 container format. One of mkv, mp4, ogg,
                                 webm, flv. Ignored if no merge is required
</code></pre>
<h2><a id="user-content-subtitle-options" class="anchor" href="#subtitle-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Subtitle Options:</h2>
<pre><code>--write-sub                      Write subtitle file
--write-auto-sub                 Write automatically generated subtitle file
                                 (YouTube only)
--all-subs                       Download all the available subtitles of the
                                 video
--list-subs                      List all available subtitles for the video
--sub-format FORMAT              Subtitle format, accepts formats
                                 preference, for example: "srt" or
                                 "ass/srt/best"
--sub-lang LANGS                 Languages of the subtitles to download
                                 (optional) separated by commas, use --list-
                                 subs for available language tags
</code></pre>
<h2><a id="user-content-authentication-options" class="anchor" href="#authentication-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Authentication Options:</h2>
<pre><code>-u, --username USERNAME          Login with this account ID
-p, --password PASSWORD          Account password. If this option is left
                                 out, youtube-dl will ask interactively.
-2, --twofactor TWOFACTOR        Two-factor authentication code
-n, --netrc                      Use .netrc authentication data
--video-password PASSWORD        Video password (vimeo, smotri, youku)
</code></pre>
<h2><a id="user-content-adobe-pass-options" class="anchor" href="#adobe-pass-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Adobe Pass Options:</h2>
<pre><code>--ap-mso MSO                     Adobe Pass multiple-system operator (TV
                                 provider) identifier, use --ap-list-mso for
                                 a list of available MSOs
--ap-username USERNAME           Multiple-system operator account login
--ap-password PASSWORD           Multiple-system operator account password.
                                 If this option is left out, youtube-dl will
                                 ask interactively.
--ap-list-mso                    List all supported multiple-system
                                 operators
</code></pre>
<h2><a id="user-content-post-processing-options" class="anchor" href="#post-processing-options" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Post-processing Options:</h2>
<pre><code>-x, --extract-audio              Convert video files to audio-only files
                                 (requires ffmpeg or avconv and ffprobe or
                                 avprobe)
--audio-format FORMAT            Specify audio format: "best", "aac",
                                 "flac", "mp3", "m4a", "opus", "vorbis", or
                                 "wav"; "best" by default; No effect without
                                 -x
--audio-quality QUALITY          Specify ffmpeg/avconv audio quality, insert
                                 a value between 0 (better) and 9 (worse)
                                 for VBR or a specific bitrate like 128K
                                 (default 5)
--recode-video FORMAT            Encode the video to another format if
                                 necessary (currently supported:
                                 mp4|flv|ogg|webm|mkv|avi)
--postprocessor-args ARGS        Give these arguments to the postprocessor
-k, --keep-video                 Keep the video file on disk after the post-
                                 processing; the video is erased by default
--no-post-overwrites             Do not overwrite post-processed files; the
                                 post-processed files are overwritten by
                                 default
--embed-subs                     Embed subtitles in the video (only for mp4,
                                 webm and mkv videos)
--embed-thumbnail                Embed thumbnail in the audio as cover art
--add-metadata                   Write metadata to the video file
--metadata-from-title FORMAT     Parse additional metadata like song title /
                                 artist from the video title. The format
                                 syntax is the same as --output. Regular
                                 expression with named capture groups may
                                 also be used. The parsed parameters replace
                                 existing values. Example: --metadata-from-
                                 title "%(artist)s - %(title)s" matches a
                                 title like "Coldplay - Paradise". Example
                                 (regex): --metadata-from-title
                                 "(?P&lt;artist&gt;.+?) - (?P&lt;title&gt;.+)"
--xattrs                         Write metadata to the video file's xattrs
                                 (using dublin core and xdg standards)
--fixup POLICY                   Automatically correct known faults of the
                                 file. One of never (do nothing), warn (only
                                 emit a warning), detect_or_warn (the
                                 default; fix file if we can, warn
                                 otherwise)
--prefer-avconv                  Prefer avconv over ffmpeg for running the
                                 postprocessors (default)
--prefer-ffmpeg                  Prefer ffmpeg over avconv for running the
                                 postprocessors
--ffmpeg-location PATH           Location of the ffmpeg/avconv binary;
                                 either the path to the binary or its
                                 containing directory.
--exec CMD                       Execute a command on the file after
                                 downloading, similar to find's -exec
                                 syntax. Example: --exec 'adb push {}
                                 /sdcard/Music/ &amp;&amp; rm {}'
--convert-subs FORMAT            Convert the subtitles to other format
                                 (currently supported: srt|ass|vtt)
</code></pre>
<h1><a id="user-content-configuration" class="anchor" href="#configuration" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>CONFIGURATION</h1>
<p>You can configure youtube-dl by placing any supported command line option to a configuration file. On Linux and OS X, the system wide configuration file is located at <code>/etc/youtube-dl.conf</code> and the user wide configuration file at <code>~/.config/youtube-dl/config</code>. On Windows, the user wide configuration file locations are <code>%APPDATA%\youtube-dl\config.txt</code> or <code>C:\Users\&lt;user name&gt;\youtube-dl.conf</code>. Note that by default configuration file may not exist so you may need to create it yourself.</p>
<p>For example, with the following configuration file youtube-dl will always extract the audio, not copy the mtime, use a proxy and save all videos under <code>Movies</code> directory in your home directory:</p>
<pre><code># Lines starting with # are comments

# Always extract audio
-x

# Do not copy the mtime
--no-mtime

# Use this proxy
--proxy 127.0.0.1:3128

# Save all videos under Movies directory in your home directory
-o ~/Movies/%(title)s.%(ext)s
</code></pre>
<p>Note that options in configuration file are just the same options aka switches used in regular command line calls thus there <strong>must be no whitespace</strong> after <code>-</code> or <code>--</code>, e.g. <code>-o</code> or <code>--proxy</code> but not <code>- o</code> or <code>-- proxy</code>.</p>
<p>You can use <code>--ignore-config</code> if you want to disable the configuration file for a particular youtube-dl run.</p>
<p>You can also use <code>--config-location</code> if you want to use custom configuration file for a particular youtube-dl run.</p>
<h3><a id="user-content-authentication-with-netrc-file" class="anchor" href="#authentication-with-netrc-file" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Authentication with <code>.netrc</code> file</h3>
<p>You may also want to configure automatic credentials storage for extractors that support authentication (by providing login and password with <code>--username</code> and <code>--password</code>) in order not to pass credentials as command line arguments on every youtube-dl execution and prevent tracking plain text passwords in the shell command history. You can achieve this using a <a href="http://stackoverflow.com/tags/.netrc/info"><code>.netrc</code> file</a> on a per extractor basis. For that you will need to create a <code>.netrc</code> file in your <code>$HOME</code> and restrict permissions to read/write by only you:</p>
<pre><code>touch $HOME/.netrc
chmod a-rwx,u+rw $HOME/.netrc
</code></pre>
<p>After that you can add credentials for an extractor in the following format, where <em>extractor</em> is the name of the extractor in lowercase:</p>
<pre><code>machine &lt;extractor&gt; login &lt;login&gt; password &lt;password&gt;
</code></pre>
<p>For example:</p>
<pre><code>machine youtube login myaccount@gmail.com password my_youtube_password
machine twitch login my_twitch_account_name password my_twitch_password
</code></pre>
<p>To activate authentication with the <code>.netrc</code> file you should pass <code>--netrc</code> to youtube-dl or place it in the <a href="#configuration">configuration file</a>.</p>
<p>On Windows you may also need to setup the <code>%HOME%</code> environment variable manually. For example:</p>
<pre><code>set HOME=%USERPROFILE%
</code></pre>
<h1><a id="user-content-output-template" class="anchor" href="#output-template" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>OUTPUT TEMPLATE</h1>
<p>The <code>-o</code> option allows users to indicate a template for the output file names.</p>
<p><strong>tl;dr:</strong> <a href="#output-template-examples">navigate me to examples</a>.</p>
<p>The basic usage is not to set any template arguments when downloading a single file, like in <code>youtube-dl -o funny_video.flv "http://some/video"</code>. However, it may contain special sequences that will be replaced when downloading each video. The special sequences may be formatted according to <a href="https://docs.python.org/2/library/stdtypes.html#string-formatting">python string formatting operations</a>. For example, <code>%(NAME)s</code> or <code>%(NAME)05d</code>. To clarify, that is a percent symbol followed by a name in parentheses, followed by a formatting operations. Allowed names along with sequence type are:</p>
<ul>
<li><code>id</code> (string): Video identifier</li>
<li><code>title</code> (string): Video title</li>
<li><code>url</code> (string): Video URL</li>
<li><code>ext</code> (string): Video filename extension</li>
<li><code>alt_title</code> (string): A secondary title of the video</li>
<li><code>display_id</code> (string): An alternative identifier for the video</li>
<li><code>uploader</code> (string): Full name of the video uploader</li>
<li><code>license</code> (string): License name the video is licensed under</li>
<li><code>creator</code> (string): The creator of the video</li>
<li><code>release_date</code> (string): The date (YYYYMMDD) when the video was released</li>
<li><code>timestamp</code> (numeric): UNIX timestamp of the moment the video became available</li>
<li><code>upload_date</code> (string): Video upload date (YYYYMMDD)</li>
<li><code>uploader_id</code> (string): Nickname or id of the video uploader</li>
<li><code>location</code> (string): Physical location where the video was filmed</li>
<li><code>duration</code> (numeric): Length of the video in seconds</li>
<li><code>view_count</code> (numeric): How many users have watched the video on the platform</li>
<li><code>like_count</code> (numeric): Number of positive ratings of the video</li>
<li><code>dislike_count</code> (numeric): Number of negative ratings of the video</li>
<li><code>repost_count</code> (numeric): Number of reposts of the video</li>
<li><code>average_rating</code> (numeric): Average rating give by users, the scale used depends on the webpage</li>
<li><code>comment_count</code> (numeric): Number of comments on the video</li>
<li><code>age_limit</code> (numeric): Age restriction for the video (years)</li>
<li><code>format</code> (string): A human-readable description of the format</li>
<li><code>format_id</code> (string): Format code specified by <code>--format</code></li>
<li><code>format_note</code> (string): Additional info about the format</li>
<li><code>width</code> (numeric): Width of the video</li>
<li><code>height</code> (numeric): Height of the video</li>
<li><code>resolution</code> (string): Textual description of width and height</li>
<li><code>tbr</code> (numeric): Average bitrate of audio and video in KBit/s</li>
<li><code>abr</code> (numeric): Average audio bitrate in KBit/s</li>
<li><code>acodec</code> (string): Name of the audio codec in use</li>
<li><code>asr</code> (numeric): Audio sampling rate in Hertz</li>
<li><code>vbr</code> (numeric): Average video bitrate in KBit/s</li>
<li><code>fps</code> (numeric): Frame rate</li>
<li><code>vcodec</code> (string): Name of the video codec in use</li>
<li><code>container</code> (string): Name of the container format</li>
<li><code>filesize</code> (numeric): The number of bytes, if known in advance</li>
<li><code>filesize_approx</code> (numeric): An estimate for the number of bytes</li>
<li><code>protocol</code> (string): The protocol that will be used for the actual download</li>
<li><code>extractor</code> (string): Name of the extractor</li>
<li><code>extractor_key</code> (string): Key name of the extractor</li>
<li><code>epoch</code> (numeric): Unix epoch when creating the file</li>
<li><code>autonumber</code> (numeric): Five-digit number that will be increased with each download, starting at zero</li>
<li><code>playlist</code> (string): Name or id of the playlist that contains the video</li>
<li><code>playlist_index</code> (numeric): Index of the video in the playlist padded with leading zeros according to the total length of the playlist</li>
<li><code>playlist_id</code> (string): Playlist identifier</li>
<li><code>playlist_title</code> (string): Playlist title</li>
</ul>
<p>Available for the video that belongs to some logical chapter or section:</p>
<ul>
<li><code>chapter</code> (string): Name or title of the chapter the video belongs to</li>
<li><code>chapter_number</code> (numeric): Number of the chapter the video belongs to</li>
<li><code>chapter_id</code> (string): Id of the chapter the video belongs to</li>
</ul>
<p>Available for the video that is an episode of some series or programme:</p>
<ul>
<li><code>series</code> (string): Title of the series or programme the video episode belongs to</li>
<li><code>season</code> (string): Title of the season the video episode belongs to</li>
<li><code>season_number</code> (numeric): Number of the season the video episode belongs to</li>
<li><code>season_id</code> (string): Id of the season the video episode belongs to</li>
<li><code>episode</code> (string): Title of the video episode</li>
<li><code>episode_number</code> (numeric): Number of the video episode within a season</li>
<li><code>episode_id</code> (string): Id of the video episode</li>
</ul>
<p>Available for the media that is a track or a part of a music album:</p>
<ul>
<li><code>track</code> (string): Title of the track</li>
<li><code>track_number</code> (numeric): Number of the track within an album or a disc</li>
<li><code>track_id</code> (string): Id of the track</li>
<li><code>artist</code> (string): Artist(s) of the track</li>
<li><code>genre</code> (string): Genre(s) of the track</li>
<li><code>album</code> (string): Title of the album the track belongs to</li>
<li><code>album_type</code> (string): Type of the album</li>
<li><code>album_artist</code> (string): List of all artists appeared on the album</li>
<li><code>disc_number</code> (numeric): Number of the disc or other physical medium the track belongs to</li>
<li><code>release_year</code> (numeric): Year (YYYY) when the album was released</li>
</ul>
<p>Each aforementioned sequence when referenced in an output template will be replaced by the actual value corresponding to the sequence name. Note that some of the sequences are not guaranteed to be present since they depend on the metadata obtained by a particular extractor. Such sequences will be replaced with <code>NA</code>.</p>
<p>For example for <code>-o %(title)s-%(id)s.%(ext)s</code> and an mp4 video with title <code>youtube-dl test video</code> and id <code>BaW_jenozKcj</code>, this will result in a <code>youtube-dl test video-BaW_jenozKcj.mp4</code> file created in the current directory.</p>
<p>For numeric sequences you can use numeric related formatting, for example, <code>%(view_count)05d</code> will result in a string with view count padded with zeros up to 5 characters, like in <code>00042</code>.</p>
<p>Output templates can also contain arbitrary hierarchical path, e.g. <code>-o '%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s'</code> which will result in downloading each video in a directory corresponding to this path template. Any missing directory will be automatically created for you.</p>
<p>To use percent literals in an output template use <code>%%</code>. To output to stdout use <code>-o -</code>.</p>
<p>The current default template is <code>%(title)s-%(id)s.%(ext)s</code>.</p>
<p>In some cases, you don't want special characters such as 中, spaces, or &amp;, such as when transferring the downloaded filename to a Windows system or the filename through an 8bit-unsafe channel. In these cases, add the <code>--restrict-filenames</code> flag to get a shorter title:</p>
<h4><a id="user-content-output-template-and-windows-batch-files" class="anchor" href="#output-template-and-windows-batch-files" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Output template and Windows batch files</h4>
<p>If you are using an output template inside a Windows batch file then you must escape plain percent characters (<code>%</code>) by doubling, so that <code>-o "%(title)s-%(id)s.%(ext)s"</code> should become <code>-o "%%(title)s-%%(id)s.%%(ext)s"</code>. However you should not touch <code>%</code>'s that are not plain characters, e.g. environment variables for expansion should stay intact: <code>-o "C:\%HOMEPATH%\Desktop\%%(title)s.%%(ext)s"</code>.</p>
<h4><a id="user-content-output-template-examples" class="anchor" href="#output-template-examples" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Output template examples</h4>
<p>Note on Windows you may need to use double quotes instead of single.</p>
<div class="highlight highlight-source-shell"><pre>$ youtube-dl --get-filename -o <span class="pl-s"><span class="pl-pds">'</span>%(title)s.%(ext)s<span class="pl-pds">'</span></span> BaW_jenozKc
youtube-dl <span class="pl-c1">test</span> video <span class="pl-s"><span class="pl-pds">'</span><span class="pl-pds">'</span></span>_ä↭𝕐.mp4    <span class="pl-c"><span class="pl-c">#</span> All kinds of weird characters</span>

$ youtube-dl --get-filename -o <span class="pl-s"><span class="pl-pds">'</span>%(title)s.%(ext)s<span class="pl-pds">'</span></span> BaW_jenozKc --restrict-filenames
youtube-dl_test_video_.mp4          <span class="pl-c"><span class="pl-c">#</span> A simple file name</span>

<span class="pl-c"><span class="pl-c">#</span> Download YouTube playlist videos in separate directory indexed by video order in a playlist</span>
$ youtube-dl -o <span class="pl-s"><span class="pl-pds">'</span>%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s<span class="pl-pds">'</span></span> https://www.youtube.com/playlist<span class="pl-k">?</span>list=PLwiyx1dc3P2JR9N8gQaQN_BCvlSlap7re

<span class="pl-c"><span class="pl-c">#</span> Download all playlists of YouTube channel/user keeping each playlist in separate directory:</span>
$ youtube-dl -o <span class="pl-s"><span class="pl-pds">'</span>%(uploader)s/%(playlist)s/%(playlist_index)s - %(title)s.%(ext)s<span class="pl-pds">'</span></span> https://www.youtube.com/user/TheLinuxFoundation/playlists

<span class="pl-c"><span class="pl-c">#</span> Download Udemy course keeping each chapter in separate directory under MyVideos directory in your home</span>
$ youtube-dl -u user -p password -o <span class="pl-s"><span class="pl-pds">'</span>~/MyVideos/%(playlist)s/%(chapter_number)s - %(chapter)s/%(title)s.%(ext)s<span class="pl-pds">'</span></span> https://www.udemy.com/java-tutorial/

<span class="pl-c"><span class="pl-c">#</span> Download entire series season keeping each series and each season in separate directory under C:/MyVideos</span>
$ youtube-dl -o <span class="pl-s"><span class="pl-pds">"</span>C:/MyVideos/%(series)s/%(season_number)s - %(season)s/%(episode_number)s - %(episode)s.%(ext)s<span class="pl-pds">"</span></span> http://videomore.ru/kino_v_detalayah/5_sezon/367617

<span class="pl-c"><span class="pl-c">#</span> Stream the video being downloaded to stdout</span>
$ youtube-dl -o - BaW_jenozKc</pre></div>
<h1><a id="user-content-format-selection" class="anchor" href="#format-selection" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>FORMAT SELECTION</h1>
<p>By default youtube-dl tries to download the best available quality, i.e. if you want the best quality you <strong>don't need</strong> to pass any special options, youtube-dl will guess it for you by <strong>default</strong>.</p>
<p>But sometimes you may want to download in a different format, for example when you are on a slow or intermittent connection. The key mechanism for achieving this is so-called <em>format selection</em> based on which you can explicitly specify desired format, select formats based on some criterion or criteria, setup precedence and much more.</p>
<p>The general syntax for format selection is <code>--format FORMAT</code> or shorter <code>-f FORMAT</code> where <code>FORMAT</code> is a <em>selector expression</em>, i.e. an expression that describes format or formats you would like to download.</p>
<p><strong>tl;dr:</strong> <a href="#format-selection-examples">navigate me to examples</a>.</p>
<p>The simplest case is requesting a specific format, for example with <code>-f 22</code> you can download the format with format code equal to 22. You can get the list of available format codes for particular video using <code>--list-formats</code> or <code>-F</code>. Note that these format codes are extractor specific.</p>
<p>You can also use a file extension (currently <code>3gp</code>, <code>aac</code>, <code>flv</code>, <code>m4a</code>, <code>mp3</code>, <code>mp4</code>, <code>ogg</code>, <code>wav</code>, <code>webm</code> are supported) to download the best quality format of a particular file extension served as a single file, e.g. <code>-f webm</code> will download the best quality format with the <code>webm</code> extension served as a single file.</p>
<p>You can also use special names to select particular edge case formats:</p>
<ul>
<li><code>best</code>: Select the best quality format represented by a single file with video and audio.</li>
<li><code>worst</code>: Select the worst quality format represented by a single file with video and audio.</li>
<li><code>bestvideo</code>: Select the best quality video-only format (e.g. DASH video). May not be available.</li>
<li><code>worstvideo</code>: Select the worst quality video-only format. May not be available.</li>
<li><code>bestaudio</code>: Select the best quality audio only-format. May not be available.</li>
<li><code>worstaudio</code>: Select the worst quality audio only-format. May not be available.</li>
</ul>
<p>For example, to download the worst quality video-only format you can use <code>-f worstvideo</code>.</p>
<p>If you want to download multiple videos and they don't have the same formats available, you can specify the order of preference using slashes. Note that slash is left-associative, i.e. formats on the left hand side are preferred, for example <code>-f 22/17/18</code> will download format 22 if it's available, otherwise it will download format 17 if it's available, otherwise it will download format 18 if it's available, otherwise it will complain that no suitable formats are available for download.</p>
<p>If you want to download several formats of the same video use a comma as a separator, e.g. <code>-f 22,17,18</code> will download all these three formats, of course if they are available. Or a more sophisticated example combined with the precedence feature: <code>-f 136/137/mp4/bestvideo,140/m4a/bestaudio</code>.</p>
<p>You can also filter the video formats by putting a condition in brackets, as in <code>-f "best[height=720]"</code> (or <code>-f "[filesize&gt;10M]"</code>).</p>
<p>The following numeric meta fields can be used with comparisons <code>&lt;</code>, <code>&lt;=</code>, <code>&gt;</code>, <code>&gt;=</code>, <code>=</code> (equals), <code>!=</code> (not equals):</p>
<ul>
<li><code>filesize</code>: The number of bytes, if known in advance</li>
<li><code>width</code>: Width of the video, if known</li>
<li><code>height</code>: Height of the video, if known</li>
<li><code>tbr</code>: Average bitrate of audio and video in KBit/s</li>
<li><code>abr</code>: Average audio bitrate in KBit/s</li>
<li><code>vbr</code>: Average video bitrate in KBit/s</li>
<li><code>asr</code>: Audio sampling rate in Hertz</li>
<li><code>fps</code>: Frame rate</li>
</ul>
<p>Also filtering work for comparisons <code>=</code> (equals), <code>!=</code> (not equals), <code>^=</code> (begins with), <code>$=</code> (ends with), <code>*=</code> (contains) and following string meta fields:</p>
<ul>
<li><code>ext</code>: File extension</li>
<li><code>acodec</code>: Name of the audio codec in use</li>
<li><code>vcodec</code>: Name of the video codec in use</li>
<li><code>container</code>: Name of the container format</li>
<li><code>protocol</code>: The protocol that will be used for the actual download, lower-case (<code>http</code>, <code>https</code>, <code>rtsp</code>, <code>rtmp</code>, <code>rtmpe</code>, <code>mms</code>, <code>f4m</code>, <code>ism</code>, <code>http_dash_segments</code>, <code>m3u8</code>, or <code>m3u8_native</code>)</li>
<li><code>format_id</code>: A short description of the format</li>
</ul>
<p>Note that none of the aforementioned meta fields are guaranteed to be present since this solely depends on the metadata obtained by particular extractor, i.e. the metadata offered by the video hoster.</p>
<p>Formats for which the value is not known are excluded unless you put a question mark (<code>?</code>) after the operator. You can combine format filters, so <code>-f "[height &lt;=? 720][tbr&gt;500]"</code> selects up to 720p videos (or videos where the height is not known) with a bitrate of at least 500 KBit/s.</p>
<p>You can merge the video and audio of two formats into a single file using <code>-f &lt;video-format&gt;+&lt;audio-format&gt;</code> (requires ffmpeg or avconv installed), for example <code>-f bestvideo+bestaudio</code> will download the best video-only format, the best audio-only format and mux them together with ffmpeg/avconv.</p>
<p>Format selectors can also be grouped using parentheses, for example if you want to download the best mp4 and webm formats with a height lower than 480 you can use <code>-f '(mp4,webm)[height&lt;480]'</code>.</p>
<p>Since the end of April 2015 and version 2015.04.26, youtube-dl uses <code>-f bestvideo+bestaudio/best</code> as the default format selection (see <a href="https://github.com/rg3/youtube-dl/issues/5447">#5447</a>, <a href="https://github.com/rg3/youtube-dl/issues/5456">#5456</a>). If ffmpeg or avconv are installed this results in downloading <code>bestvideo</code> and <code>bestaudio</code> separately and muxing them together into a single file giving the best overall quality available. Otherwise it falls back to <code>best</code> and results in downloading the best available quality served as a single file. <code>best</code> is also needed for videos that don't come from YouTube because they don't provide the audio and video in two different files. If you want to only download some DASH formats (for example if you are not interested in getting videos with a resolution higher than 1080p), you can add <code>-f bestvideo[height&lt;=?1080]+bestaudio/best</code> to your configuration file. Note that if you use youtube-dl to stream to <code>stdout</code> (and most likely to pipe it to your media player then), i.e. you explicitly specify output template as <code>-o -</code>, youtube-dl still uses <code>-f best</code> format selection in order to start content delivery immediately to your player and not to wait until <code>bestvideo</code> and <code>bestaudio</code> are downloaded and muxed.</p>
<p>If you want to preserve the old format selection behavior (prior to youtube-dl 2015.04.26), i.e. you want to download the best available quality media served as a single file, you should explicitly specify your choice with <code>-f best</code>. You may want to add it to the <a href="#configuration">configuration file</a> in order not to type it every time you run youtube-dl.</p>
<h4><a id="user-content-format-selection-examples" class="anchor" href="#format-selection-examples" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Format selection examples</h4>
<p>Note on Windows you may need to use double quotes instead of single.</p>
<div class="highlight highlight-source-shell"><pre><span class="pl-c"><span class="pl-c">#</span> Download best mp4 format available or any other best if no mp4 available</span>
$ youtube-dl -f <span class="pl-s"><span class="pl-pds">'</span>bestvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best<span class="pl-pds">'</span></span>

<span class="pl-c"><span class="pl-c">#</span> Download best format available but not better that 480p</span>
$ youtube-dl -f <span class="pl-s"><span class="pl-pds">'</span>bestvideo[height&lt;=480]+bestaudio/best[height&lt;=480]<span class="pl-pds">'</span></span>

<span class="pl-c"><span class="pl-c">#</span> Download best video only format but no bigger than 50 MB</span>
$ youtube-dl -f <span class="pl-s"><span class="pl-pds">'</span>best[filesize&lt;50M]<span class="pl-pds">'</span></span>

<span class="pl-c"><span class="pl-c">#</span> Download best format available via direct link over HTTP/HTTPS protocol</span>
$ youtube-dl -f <span class="pl-s"><span class="pl-pds">'</span>(bestvideo+bestaudio/best)[protocol^=http]<span class="pl-pds">'</span></span>

<span class="pl-c"><span class="pl-c">#</span> Download the best video format and the best audio format without merging them</span>
$ youtube-dl -f <span class="pl-s"><span class="pl-pds">'</span>bestvideo,bestaudio<span class="pl-pds">'</span></span> -o <span class="pl-s"><span class="pl-pds">'</span>%(title)s.f%(format_id)s.%(ext)s<span class="pl-pds">'</span></span></pre></div>
<p>Note that in the last example, an output template is recommended as bestvideo and bestaudio may have the same file name.</p>
<h1><a id="user-content-video-selection-1" class="anchor" href="#video-selection-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>VIDEO SELECTION</h1>
<p>Videos can be filtered by their upload date using the options <code>--date</code>, <code>--datebefore</code> or <code>--dateafter</code>. They accept dates in two formats:</p>
<ul>
<li>Absolute dates: Dates in the format <code>YYYYMMDD</code>.</li>
<li>Relative dates: Dates in the format <code>(now|today)[+-][0-9](day|week|month|year)(s)?</code></li>
</ul>
<p>Examples:</p>
<div class="highlight highlight-source-shell"><pre><span class="pl-c"><span class="pl-c">#</span> Download only the videos uploaded in the last 6 months</span>
$ youtube-dl --dateafter now-6months

<span class="pl-c"><span class="pl-c">#</span> Download only the videos uploaded on January 1, 1970</span>
$ youtube-dl --date 19700101

$ <span class="pl-c"><span class="pl-c">#</span> Download only the videos uploaded in the 200x decade</span>
$ youtube-dl --dateafter 20000101 --datebefore 20091231</pre></div>
<h1><a id="user-content-faq" class="anchor" href="#faq" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>FAQ</h1>
<h3><a id="user-content-how-do-i-update-youtube-dl" class="anchor" href="#how-do-i-update-youtube-dl" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How do I update youtube-dl?</h3>
<p>If you've followed <a href="http://rg3.github.io/youtube-dl/download.html">our manual installation instructions</a>, you can simply run <code>youtube-dl -U</code> (or, on Linux, <code>sudo youtube-dl -U</code>).</p>
<p>If you have used pip, a simple <code>sudo pip install -U youtube-dl</code> is sufficient to update.</p>
<p>If you have installed youtube-dl using a package manager like <em>apt-get</em> or <em>yum</em>, use the standard system update mechanism to update. Note that distribution packages are often outdated. As a rule of thumb, youtube-dl releases at least once a month, and often weekly or even daily. Simply go to <a href="http://yt-dl.org/">http://yt-dl.org/</a> to find out the current version. Unfortunately, there is nothing we youtube-dl developers can do if your distribution serves a really outdated version. You can (and should) complain to your distribution in their bugtracker or support forum.</p>
<p>As a last resort, you can also uninstall the version installed by your package manager and follow our manual installation instructions. For that, remove the distribution's package, with a line like</p>
<pre><code>sudo apt-get remove -y youtube-dl
</code></pre>
<p>Afterwards, simply follow <a href="http://rg3.github.io/youtube-dl/download.html">our manual installation instructions</a>:</p>
<pre><code>sudo wget https://yt-dl.org/latest/youtube-dl -O /usr/local/bin/youtube-dl
sudo chmod a+x /usr/local/bin/youtube-dl
hash -r
</code></pre>
<p>Again, from then on you'll be able to update with <code>sudo youtube-dl -U</code>.</p>
<h3><a id="user-content-youtube-dl-is-extremely-slow-to-start-on-windows" class="anchor" href="#youtube-dl-is-extremely-slow-to-start-on-windows" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>youtube-dl is extremely slow to start on Windows</h3>
<p>Add a file exclusion for <code>youtube-dl.exe</code> in Windows Defender settings.</p>
<h3><a id="user-content-im-getting-an-error-unable-to-extract-opengraph-title-on-youtube-playlists" class="anchor" href="#im-getting-an-error-unable-to-extract-opengraph-title-on-youtube-playlists" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>I'm getting an error <code>Unable to extract OpenGraph title</code> on YouTube playlists</h3>
<p>YouTube changed their playlist format in March 2014 and later on, so you'll need at least youtube-dl 2014.07.25 to download all YouTube videos.</p>
<p>If you have installed youtube-dl with a package manager, pip, setup.py or a tarball, please use that to update. Note that Ubuntu packages do not seem to get updated anymore. Since we are not affiliated with Ubuntu, there is little we can do. Feel free to <a href="https://bugs.launchpad.net/ubuntu/+source/youtube-dl/+filebug">report bugs</a> to the <a href="mailto:ubuntu-motu@lists.ubuntu.com?subject=outdated%20version%20of%20youtube-dl">Ubuntu packaging people</a> - all they have to do is update the package to a somewhat recent version. See above for a way to update.</p>
<h3><a id="user-content-im-getting-an-error-when-trying-to-use-output-template-error-using-output-template-conflicts-with-using-title-video-id-or-auto-number" class="anchor" href="#im-getting-an-error-when-trying-to-use-output-template-error-using-output-template-conflicts-with-using-title-video-id-or-auto-number" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>I'm getting an error when trying to use output template: <code>error: using output template conflicts with using title, video ID or auto number</code></h3>
<p>Make sure you are not using <code>-o</code> with any of these options <code>-t</code>, <code>--title</code>, <code>--id</code>, <code>-A</code> or <code>--auto-number</code> set in command line or in a configuration file. Remove the latter if any.</p>
<h3><a id="user-content-do-i-always-have-to-pass--citw" class="anchor" href="#do-i-always-have-to-pass--citw" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Do I always have to pass <code>-citw</code>?</h3>
<p>By default, youtube-dl intends to have the best options (incidentally, if you have a convincing case that these should be different, <a href="https://yt-dl.org/bug">please file an issue where you explain that</a>). Therefore, it is unnecessary and sometimes harmful to copy long option strings from webpages. In particular, the only option out of <code>-citw</code> that is regularly useful is <code>-i</code>.</p>
<h3><a id="user-content-can-you-please-put-the--b-option-back" class="anchor" href="#can-you-please-put-the--b-option-back" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Can you please put the <code>-b</code> option back?</h3>
<p>Most people asking this question are not aware that youtube-dl now defaults to downloading the highest available quality as reported by YouTube, which will be 1080p or 720p in some cases, so you no longer need the <code>-b</code> option. For some specific videos, maybe YouTube does not report them to be available in a specific high quality format you're interested in. In that case, simply request it with the <code>-f</code> option and youtube-dl will try to download it.</p>
<h3><a id="user-content-i-get-http-error-402-when-trying-to-download-a-video-whats-this" class="anchor" href="#i-get-http-error-402-when-trying-to-download-a-video-whats-this" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>I get HTTP error 402 when trying to download a video. What's this?</h3>
<p>Apparently YouTube requires you to pass a CAPTCHA test if you download too much. We're <a href="https://github.com/rg3/youtube-dl/issues/154">considering to provide a way to let you solve the CAPTCHA</a>, but at the moment, your best course of action is pointing a web browser to the youtube URL, solving the CAPTCHA, and restart youtube-dl.</p>
<h3><a id="user-content-do-i-need-any-other-programs" class="anchor" href="#do-i-need-any-other-programs" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Do I need any other programs?</h3>
<p>youtube-dl works fine on its own on most sites. However, if you want to convert video/audio, you'll need <a href="https://libav.org/">avconv</a> or <a href="https://www.ffmpeg.org/">ffmpeg</a>. On some sites - most notably YouTube - videos can be retrieved in a higher quality format without sound. youtube-dl will detect whether avconv/ffmpeg is present and automatically pick the best option.</p>
<p>Videos or video formats streamed via RTMP protocol can only be downloaded when <a href="https://rtmpdump.mplayerhq.hu/">rtmpdump</a> is installed. Downloading MMS and RTSP videos requires either <a href="http://mplayerhq.hu/">mplayer</a> or <a href="https://mpv.io/">mpv</a> to be installed.</p>
<h3><a id="user-content-i-have-downloaded-a-video-but-how-can-i-play-it" class="anchor" href="#i-have-downloaded-a-video-but-how-can-i-play-it" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>I have downloaded a video but how can I play it?</h3>
<p>Once the video is fully downloaded, use any video player, such as <a href="https://mpv.io/">mpv</a>, <a href="http://www.videolan.org/">vlc</a> or <a href="http://www.mplayerhq.hu/">mplayer</a>.</p>
<h3><a id="user-content-i-extracted-a-video-url-with--g-but-it-does-not-play-on-another-machine--in-my-web-browser" class="anchor" href="#i-extracted-a-video-url-with--g-but-it-does-not-play-on-another-machine--in-my-web-browser" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>I extracted a video URL with <code>-g</code>, but it does not play on another machine / in my web browser.</h3>
<p>It depends a lot on the service. In many cases, requests for the video (to download/play it) must come from the same IP address and with the same cookies and/or HTTP headers. Use the <code>--cookies</code> option to write the required cookies into a file, and advise your downloader to read cookies from that file. Some sites also require a common user agent to be used, use <code>--dump-user-agent</code> to see the one in use by youtube-dl. You can also get necessary cookies and HTTP headers from JSON output obtained with <code>--dump-json</code>.</p>
<p>It may be beneficial to use IPv6; in some cases, the restrictions are only applied to IPv4. Some services (sometimes only for a subset of videos) do not restrict the video URL by IP address, cookie, or user-agent, but these are the exception rather than the rule.</p>
<p>Please bear in mind that some URL protocols are <strong>not</strong> supported by browsers out of the box, including RTMP. If you are using <code>-g</code>, your own downloader must support these as well.</p>
<p>If you want to play the video on a machine that is not running youtube-dl, you can relay the video content from the machine that runs youtube-dl. You can use <code>-o -</code> to let youtube-dl stream a video to stdout, or simply allow the player to download the files written by youtube-dl in turn.</p>
<h3><a id="user-content-error-no-fmt_url_map-or-conn-information-found-in-video-info" class="anchor" href="#error-no-fmt_url_map-or-conn-information-found-in-video-info" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ERROR: no fmt_url_map or conn information found in video info</h3>
<p>YouTube has switched to a new video info format in July 2011 which is not supported by old versions of youtube-dl. See <a href="#how-do-i-update-youtube-dl">above</a> for how to update youtube-dl.</p>
<h3><a id="user-content-error-unable-to-download-video" class="anchor" href="#error-unable-to-download-video" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ERROR: unable to download video</h3>
<p>YouTube requires an additional signature since September 2012 which is not supported by old versions of youtube-dl. See <a href="#how-do-i-update-youtube-dl">above</a> for how to update youtube-dl.</p>
<h3><a id="user-content-video-url-contains-an-ampersand-and-im-getting-some-strange-output-1-2839-or-v-is-not-recognized-as-an-internal-or-external-command" class="anchor" href="#video-url-contains-an-ampersand-and-im-getting-some-strange-output-1-2839-or-v-is-not-recognized-as-an-internal-or-external-command" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Video URL contains an ampersand and I'm getting some strange output <code>[1] 2839</code> or <code>'v' is not recognized as an internal or external command</code></h3>
<p>That's actually the output from your shell. Since ampersand is one of the special shell characters it's interpreted by the shell preventing you from passing the whole URL to youtube-dl. To disable your shell from interpreting the ampersands (or any other special characters) you have to either put the whole URL in quotes or escape them with a backslash (which approach will work depends on your shell).</p>
<p>For example if your URL is <a href="https://www.youtube.com/watch?t=4&amp;v=BaW_jenozKc">https://www.youtube.com/watch?t=4&amp;v=BaW_jenozKc</a> you should end up with following command:</p>
<p><code>youtube-dl 'https://www.youtube.com/watch?t=4&amp;v=BaW_jenozKc'</code></p>
<p>or</p>
<p><code>youtube-dl https://www.youtube.com/watch?t=4\&amp;v=BaW_jenozKc</code></p>
<p>For Windows you have to use the double quotes:</p>
<p><code>youtube-dl "https://www.youtube.com/watch?t=4&amp;v=BaW_jenozKc"</code></p>
<h3><a id="user-content-extractorerror-could-not-find-js-function-uof" class="anchor" href="#extractorerror-could-not-find-js-function-uof" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>ExtractorError: Could not find JS function u'OF'</h3>
<p>In February 2015, the new YouTube player contained a character sequence in a string that was misinterpreted by old versions of youtube-dl. See <a href="#how-do-i-update-youtube-dl">above</a> for how to update youtube-dl.</p>
<h3><a id="user-content-http-error-429-too-many-requests-or-402-payment-required" class="anchor" href="#http-error-429-too-many-requests-or-402-payment-required" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>HTTP Error 429: Too Many Requests or 402: Payment Required</h3>
<p>These two error codes indicate that the service is blocking your IP address because of overuse. Contact the service and ask them to unblock your IP address, or - if you have acquired a whitelisted IP address already - use the <a href="#network-options"><code>--proxy</code> or <code>--source-address</code> options</a> to select another IP address.</p>
<h3><a id="user-content-syntaxerror-non-ascii-character" class="anchor" href="#syntaxerror-non-ascii-character" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>SyntaxError: Non-ASCII character</h3>
<p>The error</p>
<pre><code>File "youtube-dl", line 2
SyntaxError: Non-ASCII character '\x93' ...
</code></pre>
<p>means you're using an outdated version of Python. Please update to Python 2.6 or 2.7.</p>
<h3><a id="user-content-what-is-this-binary-file-where-has-the-code-gone" class="anchor" href="#what-is-this-binary-file-where-has-the-code-gone" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>What is this binary file? Where has the code gone?</h3>
<p>Since June 2012 (<a href="https://github.com/rg3/youtube-dl/issues/342">#342</a>) youtube-dl is packed as an executable zipfile, simply unzip it (might need renaming to <code>youtube-dl.zip</code> first on some systems) or clone the git repository, as laid out above. If you modify the code, you can run it by executing the <code>__main__.py</code> file. To recompile the executable, run <code>make youtube-dl</code>.</p>
<h3><a id="user-content-the-exe-throws-an-error-due-to-missing-msvcr100dll" class="anchor" href="#the-exe-throws-an-error-due-to-missing-msvcr100dll" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>The exe throws an error due to missing <code>MSVCR100.dll</code></h3>
<p>To run the exe you need to install first the <a href="https://www.microsoft.com/en-US/download/details.aspx?id=5555">Microsoft Visual C++ 2010 Redistributable Package (x86)</a>.</p>
<h3><a id="user-content-on-windows-how-should-i-set-up-ffmpeg-and-youtube-dl-where-should-i-put-the-exe-files" class="anchor" href="#on-windows-how-should-i-set-up-ffmpeg-and-youtube-dl-where-should-i-put-the-exe-files" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>On Windows, how should I set up ffmpeg and youtube-dl? Where should I put the exe files?</h3>
<p>If you put youtube-dl and ffmpeg in the same directory that you're running the command from, it will work, but that's rather cumbersome.</p>
<p>To make a different directory work - either for ffmpeg, or for youtube-dl, or for both - simply create the directory (say, <code>C:\bin</code>, or <code>C:\Users\&lt;User name&gt;\bin</code>), put all the executables directly in there, and then <a href="https://www.java.com/en/download/help/path.xml">set your PATH environment variable</a> to include that directory.</p>
<p>From then on, after restarting your shell, you will be able to access both youtube-dl and ffmpeg (and youtube-dl will be able to find ffmpeg) by simply typing <code>youtube-dl</code> or <code>ffmpeg</code>, no matter what directory you're in.</p>
<h3><a id="user-content-how-do-i-put-downloads-into-a-specific-folder" class="anchor" href="#how-do-i-put-downloads-into-a-specific-folder" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How do I put downloads into a specific folder?</h3>
<p>Use the <code>-o</code> to specify an <a href="#output-template">output template</a>, for example <code>-o "/home/user/videos/%(title)s-%(id)s.%(ext)s"</code>. If you want this for all of your downloads, put the option into your <a href="#configuration">configuration file</a>.</p>
<h3><a id="user-content-how-do-i-download-a-video-starting-with-a--" class="anchor" href="#how-do-i-download-a-video-starting-with-a--" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How do I download a video starting with a <code>-</code>?</h3>
<p>Either prepend <code>http://www.youtube.com/watch?v=</code> or separate the ID from the options with <code>--</code>:</p>
<pre><code>youtube-dl -- -wNyEUrxzFU
youtube-dl "http://www.youtube.com/watch?v=-wNyEUrxzFU"
</code></pre>
<h3><a id="user-content-how-do-i-pass-cookies-to-youtube-dl" class="anchor" href="#how-do-i-pass-cookies-to-youtube-dl" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How do I pass cookies to youtube-dl?</h3>
<p>Use the <code>--cookies</code> option, for example <code>--cookies /path/to/cookies/file.txt</code>.</p>
<p>In order to extract cookies from browser use any conforming browser extension for exporting cookies. For example, <a href="https://chrome.google.com/webstore/detail/cookiestxt/njabckikapfpffapmjgojcnbfjonfjfg">cookies.txt</a> (for Chrome) or <a href="https://addons.mozilla.org/en-US/firefox/addon/export-cookies/">Export Cookies</a> (for Firefox).</p>
<p>Note that the cookies file must be in Mozilla/Netscape format and the first line of the cookies file must be either <code># HTTP Cookie File</code> or <code># Netscape HTTP Cookie File</code>. Make sure you have correct <a href="https://en.wikipedia.org/wiki/Newline">newline format</a> in the cookies file and convert newlines if necessary to correspond with your OS, namely <code>CRLF</code> (<code>\r\n</code>) for Windows and <code>LF</code> (<code>\n</code>) for Unix and Unix-like systems (Linux, Mac OS, etc.). <code>HTTP Error 400: Bad Request</code> when using <code>--cookies</code> is a good sign of invalid newline format.</p>
<p>Passing cookies to youtube-dl is a good way to workaround login when a particular extractor does not implement it explicitly. Another use case is working around <a href="https://en.wikipedia.org/wiki/CAPTCHA">CAPTCHA</a> some websites require you to solve in particular cases in order to get access (e.g. YouTube, CloudFlare).</p>
<h3><a id="user-content-how-do-i-stream-directly-to-media-player" class="anchor" href="#how-do-i-stream-directly-to-media-player" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How do I stream directly to media player?</h3>
<p>You will first need to tell youtube-dl to stream media to stdout with <code>-o -</code>, and also tell your media player to read from stdin (it must be capable of this for streaming) and then pipe former to latter. For example, streaming to <a href="http://www.videolan.org/">vlc</a> can be achieved with:</p>
<pre><code>youtube-dl -o - "http://www.youtube.com/watch?v=BaW_jenozKcj" | vlc -
</code></pre>
<h3><a id="user-content-how-do-i-download-only-new-videos-from-a-playlist" class="anchor" href="#how-do-i-download-only-new-videos-from-a-playlist" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How do I download only new videos from a playlist?</h3>
<p>Use download-archive feature. With this feature you should initially download the complete playlist with <code>--download-archive /path/to/download/archive/file.txt</code> that will record identifiers of all the videos in a special file. Each subsequent run with the same <code>--download-archive</code> will download only new videos and skip all videos that have been downloaded before. Note that only successful downloads are recorded in the file.</p>
<p>For example, at first,</p>
<pre><code>youtube-dl --download-archive archive.txt "https://www.youtube.com/playlist?list=PLwiyx1dc3P2JR9N8gQaQN_BCvlSlap7re"
</code></pre>
<p>will download the complete <code>PLwiyx1dc3P2JR9N8gQaQN_BCvlSlap7re</code> playlist and create a file <code>archive.txt</code>. Each subsequent run will only download new videos if any:</p>
<pre><code>youtube-dl --download-archive archive.txt "https://www.youtube.com/playlist?list=PLwiyx1dc3P2JR9N8gQaQN_BCvlSlap7re"
</code></pre>
<h3><a id="user-content-should-i-add---hls-prefer-native-into-my-config" class="anchor" href="#should-i-add---hls-prefer-native-into-my-config" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Should I add <code>--hls-prefer-native</code> into my config?</h3>
<p>When youtube-dl detects an HLS video, it can download it either with the built-in downloader or ffmpeg. Since many HLS streams are slightly invalid and ffmpeg/youtube-dl each handle some invalid cases better than the other, there is an option to switch the downloader if needed.</p>
<p>When youtube-dl knows that one particular downloader works better for a given website, that downloader will be picked. Otherwise, youtube-dl will pick the best downloader for general compatibility, which at the moment happens to be ffmpeg. This choice may change in future versions of youtube-dl, with improvements of the built-in downloader and/or ffmpeg.</p>
<p>In particular, the generic extractor (used when your website is not in the <a href="http://rg3.github.io/youtube-dl/supportedsites.html">list of supported sites by youtube-dl</a> cannot mandate one specific downloader.</p>
<p>If you put either <code>--hls-prefer-native</code> or <code>--hls-prefer-ffmpeg</code> into your configuration, a different subset of videos will fail to download correctly. Instead, it is much better to <a href="https://yt-dl.org/bug">file an issue</a> or a pull request which details why the native or the ffmpeg HLS downloader is a better choice for your use case.</p>
<h3><a id="user-content-can-you-add-support-for-this-anime-video-site-or-site-which-shows-current-movies-for-free" class="anchor" href="#can-you-add-support-for-this-anime-video-site-or-site-which-shows-current-movies-for-free" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Can you add support for this anime video site, or site which shows current movies for free?</h3>
<p>As a matter of policy (as well as legality), youtube-dl does not include support for services that specialize in infringing copyright. As a rule of thumb, if you cannot easily find a video that the service is quite obviously allowed to distribute (i.e. that has been uploaded by the creator, the creator's distributor, or is published under a free license), the service is probably unfit for inclusion to youtube-dl.</p>
<p>A note on the service that they don't host the infringing content, but just link to those who do, is evidence that the service should <strong>not</strong> be included into youtube-dl. The same goes for any DMCA note when the whole front page of the service is filled with videos they are not allowed to distribute. A "fair use" note is equally unconvincing if the service shows copyright-protected videos in full without authorization.</p>
<p>Support requests for services that <strong>do</strong> purchase the rights to distribute their content are perfectly fine though. If in doubt, you can simply include a source that mentions the legitimate purchase of content.</p>
<h3><a id="user-content-how-can-i-speed-up-work-on-my-issue" class="anchor" href="#how-can-i-speed-up-work-on-my-issue" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How can I speed up work on my issue?</h3>
<p>(Also known as: Help, my important issue not being solved!) The youtube-dl core developer team is quite small. While we do our best to solve as many issues as possible, sometimes that can take quite a while. To speed up your issue, here's what you can do:</p>
<p>First of all, please do report the issue <a href="https://yt-dl.org/bugs">at our issue tracker</a>. That allows us to coordinate all efforts by users and developers, and serves as a unified point. Unfortunately, the youtube-dl project has grown too large to use personal email as an effective communication channel.</p>
<p>Please read the <a href="#bugs">bug reporting instructions</a> below. A lot of bugs lack all the necessary information. If you can, offer proxy, VPN, or shell access to the youtube-dl developers. If you are able to, test the issue from multiple computers in multiple countries to exclude local censorship or misconfiguration issues.</p>
<p>If nobody is interested in solving your issue, you are welcome to take matters into your own hands and submit a pull request (or coerce/pay somebody else to do so).</p>
<p>Feel free to bump the issue from time to time by writing a small comment ("Issue is still present in youtube-dl version ...from France, but fixed from Belgium"), but please not more than once a month. Please do not declare your issue as <code>important</code> or <code>urgent</code>.</p>
<h3><a id="user-content-how-can-i-detect-whether-a-given-url-is-supported-by-youtube-dl" class="anchor" href="#how-can-i-detect-whether-a-given-url-is-supported-by-youtube-dl" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>How can I detect whether a given URL is supported by youtube-dl?</h3>
<p>For one, have a look at the <a href="/rg3/youtube-dl/blob/master/docs/supportedsites.md">list of supported sites</a>. Note that it can sometimes happen that the site changes its URL scheme (say, from <a href="http://example.com/video/1234567">http://example.com/video/1234567</a> to <a href="http://example.com/v/1234567">http://example.com/v/1234567</a> ) and youtube-dl reports an URL of a service in that list as unsupported. In that case, simply report a bug.</p>
<p>It is <em>not</em> possible to detect whether a URL is supported or not. That's because youtube-dl contains a generic extractor which matches <strong>all</strong> URLs. You may be tempted to disable, exclude, or remove the generic extractor, but the generic extractor not only allows users to extract videos from lots of websites that embed a video from another service, but may also be used to extract video from a service that it's hosting itself. Therefore, we neither recommend nor support disabling, excluding, or removing the generic extractor.</p>
<p>If you want to find out whether a given URL is supported, simply call youtube-dl with it. If you get no videos back, chances are the URL is either not referring to a video or unsupported. You can find out which by examining the output (if you run youtube-dl on the console) or catching an <code>UnsupportedError</code> exception if you run it from a Python program.</p>
<h1><a id="user-content-why-do-i-need-to-go-through-that-much-red-tape-when-filing-bugs" class="anchor" href="#why-do-i-need-to-go-through-that-much-red-tape-when-filing-bugs" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Why do I need to go through that much red tape when filing bugs?</h1>
<p>Before we had the issue template, despite our extensive <a href="#bugs">bug reporting instructions</a>, about 80% of the issue reports we got were useless, for instance because people used ancient versions hundreds of releases old, because of simple syntactic errors (not in youtube-dl but in general shell usage), because the problem was already reported multiple times before, because people did not actually read an error message, even if it said "please install ffmpeg", because people did not mention the URL they were trying to download and many more simple, easy-to-avoid problems, many of whom were totally unrelated to youtube-dl.</p>
<p>youtube-dl is an open-source project manned by too few volunteers, so we'd rather spend time fixing bugs where we are certain none of those simple problems apply, and where we can be reasonably confident to be able to reproduce the issue without asking the reporter repeatedly. As such, the output of <code>youtube-dl -v YOUR_URL_HERE</code> is really all that's required to file an issue. The issue template also guides you through some basic steps you can do, such as checking that your version of youtube-dl is current.</p>
<h1><a id="user-content-developer-instructions" class="anchor" href="#developer-instructions" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>DEVELOPER INSTRUCTIONS</h1>
<p>Most users do not need to build youtube-dl and can <a href="http://rg3.github.io/youtube-dl/download.html">download the builds</a> or get them from their distribution.</p>
<p>To run youtube-dl as a developer, you don't need to build anything either. Simply execute</p>
<pre><code>python -m youtube_dl
</code></pre>
<p>To run the test, simply invoke your favorite test runner, or execute a test file directly; any of the following work:</p>
<pre><code>python -m unittest discover
python test/test_download.py
nosetests
</code></pre>
<p>If you want to create a build of youtube-dl yourself, you'll need</p>
<ul>
<li>python</li>
<li>make (only GNU make is supported)</li>
<li>pandoc</li>
<li>zip</li>
<li>nosetests</li>
</ul>
<h3><a id="user-content-adding-support-for-a-new-site" class="anchor" href="#adding-support-for-a-new-site" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Adding support for a new site</h3>
<p>If you want to add support for a new site, first of all <strong>make sure</strong> this site is <strong>not dedicated to <a href="/rg3/youtube-dl/blob/master/README.md#can-you-add-support-for-this-anime-video-site-or-site-which-shows-current-movies-for-free">copyright infringement</a></strong>. youtube-dl does <strong>not support</strong> such sites thus pull requests adding support for them <strong>will be rejected</strong>.</p>
<p>After you have ensured this site is distributing its content legally, you can follow this quick list (assuming your service is called <code>yourextractor</code>):</p>
<ol>
<li>
<p><a href="https://github.com/rg3/youtube-dl/fork">Fork this repository</a></p>
</li>
<li>
<p>Check out the source code with:</p>
<pre><code> git clone git@github.com:YOUR_GITHUB_USERNAME/youtube-dl.git
</code></pre>
</li>
<li>
<p>Start a new git branch with</p>
<pre><code> cd youtube-dl
 git checkout -b yourextractor
</code></pre>
</li>
<li>
<p>Start with this simple template and save it to <code>youtube_dl/extractor/yourextractor.py</code>:</p>
<div class="highlight highlight-source-python"><pre><span class="pl-c"><span class="pl-c">#</span> coding: utf-8</span>
<span class="pl-k">from</span> <span class="pl-c1">__future__</span> <span class="pl-k">import</span> unicode_literals

<span class="pl-k">from</span> .common <span class="pl-k">import</span> InfoExtractor


<span class="pl-k">class</span> <span class="pl-en">YourExtractorIE</span>(<span class="pl-e">InfoExtractor</span>):
    <span class="pl-c1">_VALID_URL</span> <span class="pl-k">=</span> <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>https<span class="pl-k">?</span>://(?:www<span class="pl-cce">\.</span>)<span class="pl-k">?</span>yourextractor<span class="pl-cce">\.</span>com/watch/(<span class="pl-ent">?P&lt;id&gt;</span><span class="pl-c1">[</span><span class="pl-c1">0-9</span><span class="pl-c1">]</span><span class="pl-k">+</span>)<span class="pl-pds">'</span></span>
    <span class="pl-c1">_TEST</span> <span class="pl-k">=</span> {
        <span class="pl-s"><span class="pl-pds">'</span>url<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>http://yourextractor.com/watch/42<span class="pl-pds">'</span></span>,
        <span class="pl-s"><span class="pl-pds">'</span>md5<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>TODO: md5 sum of the first 10241 bytes of the video file (use --test)<span class="pl-pds">'</span></span>,
        <span class="pl-s"><span class="pl-pds">'</span>info_dict<span class="pl-pds">'</span></span>: {
            <span class="pl-s"><span class="pl-pds">'</span>id<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>42<span class="pl-pds">'</span></span>,
            <span class="pl-s"><span class="pl-pds">'</span>ext<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>mp4<span class="pl-pds">'</span></span>,
            <span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>Video title goes here<span class="pl-pds">'</span></span>,
            <span class="pl-s"><span class="pl-pds">'</span>thumbnail<span class="pl-pds">'</span></span>: <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>re:<span class="pl-c1">^</span>https<span class="pl-k">?</span>://<span class="pl-c1">.</span><span class="pl-k">*</span><span class="pl-cce">\.</span>jpg<span class="pl-c1">$</span><span class="pl-pds">'</span></span>,
            <span class="pl-c"><span class="pl-c">#</span> <span class="pl-k">TODO</span> more properties, either as:</span>
            <span class="pl-c"><span class="pl-c">#</span> * A value</span>
            <span class="pl-c"><span class="pl-c">#</span> * MD5 checksum; start the string with md5:</span>
            <span class="pl-c"><span class="pl-c">#</span> * A regular expression; start the string with re:</span>
            <span class="pl-c"><span class="pl-c">#</span> * Any Python type (for example int or float)</span>
        }
    }

    <span class="pl-k">def</span> <span class="pl-en">_real_extract</span>(<span class="pl-smi"><span class="pl-smi">self</span></span>, <span class="pl-smi">url</span>):
        video_id <span class="pl-k">=</span> <span class="pl-c1">self</span>._match_id(url)
        webpage <span class="pl-k">=</span> <span class="pl-c1">self</span>._download_webpage(url, video_id)

        <span class="pl-c"><span class="pl-c">#</span> <span class="pl-k">TODO</span> more code goes here, for example ...</span>
        title <span class="pl-k">=</span> <span class="pl-c1">self</span>._html_search_regex(<span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;h1&gt;(<span class="pl-c1">.</span><span class="pl-k">+?</span>)&lt;/h1&gt;<span class="pl-pds">'</span></span>, webpage, <span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>)

        <span class="pl-k">return</span> {
            <span class="pl-s"><span class="pl-pds">'</span>id<span class="pl-pds">'</span></span>: video_id,
            <span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>: title,
            <span class="pl-s"><span class="pl-pds">'</span>description<span class="pl-pds">'</span></span>: <span class="pl-c1">self</span>._og_search_description(webpage),
            <span class="pl-s"><span class="pl-pds">'</span>uploader<span class="pl-pds">'</span></span>: <span class="pl-c1">self</span>._search_regex(<span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;div<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>id="uploader"<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">*</span>&gt;(<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&lt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>)&lt;<span class="pl-pds">'</span></span>, webpage, <span class="pl-s"><span class="pl-pds">'</span>uploader<span class="pl-pds">'</span></span>, <span class="pl-v">fatal</span><span class="pl-k">=</span><span class="pl-c1">False</span>),
            <span class="pl-c"><span class="pl-c">#</span> <span class="pl-k">TODO</span> more properties (see youtube_dl/extractor/common.py)</span>
        }</pre></div>
</li>
<li>
<p>Add an import in <a href="https://github.com/rg3/youtube-dl/blob/master/youtube_dl/extractor/extractors.py"><code>youtube_dl/extractor/extractors.py</code></a>.</p>
</li>
<li>
<p>Run <code>python test/test_download.py TestDownload.test_YourExtractor</code>. This <em>should fail</em> at first, but you can continually re-run it until you're done. If you decide to add more than one test, then rename <code>_TEST</code> to <code>_TESTS</code> and make it into a list of dictionaries. The tests will then be named <code>TestDownload.test_YourExtractor</code>, <code>TestDownload.test_YourExtractor_1</code>, <code>TestDownload.test_YourExtractor_2</code>, etc.</p>
</li>
<li>
<p>Have a look at <a href="https://github.com/rg3/youtube-dl/blob/master/youtube_dl/extractor/common.py"><code>youtube_dl/extractor/common.py</code></a> for possible helper methods and a <a href="https://github.com/rg3/youtube-dl/blob/master/youtube_dl/extractor/common.py#L74-L252">detailed description of what your extractor should and may return</a>. Add tests and code for as many as you want.</p>
</li>
<li>
<p>Make sure your code follows <a href="#youtube-dl-coding-conventions">youtube-dl coding conventions</a> and check the code with <a href="https://pypi.python.org/pypi/flake8">flake8</a>. Also make sure your code works under all <a href="http://www.python.org/">Python</a> versions claimed supported by youtube-dl, namely 2.6, 2.7, and 3.2+.</p>
</li>
<li>
<p>When the tests pass, <a href="http://git-scm.com/docs/git-add">add</a> the new files and <a href="http://git-scm.com/docs/git-commit">commit</a> them and <a href="http://git-scm.com/docs/git-push">push</a> the result, like this:</p>
<pre><code> $ git add youtube_dl/extractor/extractors.py
 $ git add youtube_dl/extractor/yourextractor.py
 $ git commit -m '[yourextractor] Add new extractor'
 $ git push origin yourextractor
</code></pre>
</li>
<li>
<p>Finally, <a href="https://help.github.com/articles/creating-a-pull-request">create a pull request</a>. We'll then review and merge it.</p>
</li>
</ol>
<p>In any case, thank you very much for your contributions!</p>
<h2><a id="user-content-youtube-dl-coding-conventions" class="anchor" href="#youtube-dl-coding-conventions" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>youtube-dl coding conventions</h2>
<p>This section introduces a guide lines for writing idiomatic, robust and future-proof extractor code.</p>
<p>Extractors are very fragile by nature since they depend on the layout of the source data provided by 3rd party media hosters out of your control and this layout tends to change. As an extractor implementer your task is not only to write code that will extract media links and metadata correctly but also to minimize dependency on the source's layout and even to make the code foresee potential future changes and be ready for that. This is important because it will allow the extractor not to break on minor layout changes thus keeping old youtube-dl versions working. Even though this breakage issue is easily fixed by emitting a new version of youtube-dl with a fix incorporated, all the previous versions become broken in all repositories and distros' packages that may not be so prompt in fetching the update from us. Needless to say, some non rolling release distros may never receive an update at all.</p>
<h3><a id="user-content-mandatory-and-optional-metafields" class="anchor" href="#mandatory-and-optional-metafields" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Mandatory and optional metafields</h3>
<p>For extraction to work youtube-dl relies on metadata your extractor extracts and provides to youtube-dl expressed by an <a href="https://github.com/rg3/youtube-dl/blob/master/youtube_dl/extractor/common.py#L75-L257">information dictionary</a> or simply <em>info dict</em>. Only the following meta fields in the <em>info dict</em> are considered mandatory for a successful extraction process by youtube-dl:</p>
<ul>
<li><code>id</code> (media identifier)</li>
<li><code>title</code> (media title)</li>
<li><code>url</code> (media download URL) or <code>formats</code></li>
</ul>
<p>In fact only the last option is technically mandatory (i.e. if you can't figure out the download location of the media the extraction does not make any sense). But by convention youtube-dl also treats <code>id</code> and <code>title</code> as mandatory. Thus the aforementioned metafields are the critical data that the extraction does not make any sense without and if any of them fail to be extracted then the extractor is considered completely broken.</p>
<p><a href="https://github.com/rg3/youtube-dl/blob/master/youtube_dl/extractor/common.py#L149-L257">Any field</a> apart from the aforementioned ones are considered <strong>optional</strong>. That means that extraction should be <strong>tolerant</strong> to situations when sources for these fields can potentially be unavailable (even if they are always available at the moment) and <strong>future-proof</strong> in order not to break the extraction of general purpose mandatory fields.</p>
<h4><a id="user-content-example" class="anchor" href="#example" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Example</h4>
<p>Say you have some source dictionary <code>meta</code> that you've fetched as JSON with HTTP request and it has a key <code>summary</code>:</p>
<div class="highlight highlight-source-python"><pre>meta <span class="pl-k">=</span> <span class="pl-c1">self</span>._download_json(url, video_id)</pre></div>
<p>Assume at this point <code>meta</code>'s layout is:</p>
<div class="highlight highlight-source-python"><pre>{
    <span class="pl-c1">...</span>
    <span class="pl-s"><span class="pl-pds">"</span>summary<span class="pl-pds">"</span></span>: <span class="pl-s"><span class="pl-pds">"</span>some fancy summary text<span class="pl-pds">"</span></span>,
    <span class="pl-c1">...</span>
}</pre></div>
<p>Assume you want to extract <code>summary</code> and put it into the resulting info dict as <code>description</code>. Since <code>description</code> is an optional meta field you should be ready that this key may be missing from the <code>meta</code> dict, so that you should extract it like:</p>
<div class="highlight highlight-source-python"><pre>description <span class="pl-k">=</span> meta.get(<span class="pl-s"><span class="pl-pds">'</span>summary<span class="pl-pds">'</span></span>)  <span class="pl-c"><span class="pl-c">#</span> correct</span></pre></div>
<p>and not like:</p>
<div class="highlight highlight-source-python"><pre>description <span class="pl-k">=</span> meta[<span class="pl-s"><span class="pl-pds">'</span>summary<span class="pl-pds">'</span></span>]  <span class="pl-c"><span class="pl-c">#</span> incorrect</span></pre></div>
<p>The latter will break extraction process with <code>KeyError</code> if <code>summary</code> disappears from <code>meta</code> at some later time but with the former approach extraction will just go ahead with <code>description</code> set to <code>None</code> which is perfectly fine (remember <code>None</code> is equivalent to the absence of data).</p>
<p>Similarly, you should pass <code>fatal=False</code> when extracting optional data from a webpage with <code>_search_regex</code>, <code>_html_search_regex</code> or similar methods, for instance:</p>
<div class="highlight highlight-source-python"><pre>description <span class="pl-k">=</span> <span class="pl-c1">self</span>._search_regex(
    <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;span<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>id="title"<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">*</span>&gt;(<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&lt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>)&lt;<span class="pl-pds">'</span></span>,
    webpage, <span class="pl-s"><span class="pl-pds">'</span>description<span class="pl-pds">'</span></span>, <span class="pl-v">fatal</span><span class="pl-k">=</span><span class="pl-c1">False</span>)</pre></div>
<p>With <code>fatal</code> set to <code>False</code> if <code>_search_regex</code> fails to extract <code>description</code> it will emit a warning and continue extraction.</p>
<p>You can also pass <code>default=&lt;some fallback value&gt;</code>, for example:</p>
<div class="highlight highlight-source-python"><pre>description <span class="pl-k">=</span> <span class="pl-c1">self</span>._search_regex(
    <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;span<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>id="title"<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">*</span>&gt;(<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&lt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>)&lt;<span class="pl-pds">'</span></span>,
    webpage, <span class="pl-s"><span class="pl-pds">'</span>description<span class="pl-pds">'</span></span>, <span class="pl-v">default</span><span class="pl-k">=</span><span class="pl-c1">None</span>)</pre></div>
<p>On failure this code will silently continue the extraction with <code>description</code> set to <code>None</code>. That is useful for metafields that may or may not be present.</p>
<h3><a id="user-content-provide-fallbacks" class="anchor" href="#provide-fallbacks" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Provide fallbacks</h3>
<p>When extracting metadata try to do so from multiple sources. For example if <code>title</code> is present in several places, try extracting from at least some of them. This makes it more future-proof in case some of the sources become unavailable.</p>
<h4><a id="user-content-example-1" class="anchor" href="#example-1" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Example</h4>
<p>Say <code>meta</code> from the previous example has a <code>title</code> and you are about to extract it. Since <code>title</code> is a mandatory meta field you should end up with something like:</p>
<div class="highlight highlight-source-python"><pre>title <span class="pl-k">=</span> meta[<span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>]</pre></div>
<p>If <code>title</code> disappears from <code>meta</code> in future due to some changes on the hoster's side the extraction would fail since <code>title</code> is mandatory. That's expected.</p>
<p>Assume that you have some another source you can extract <code>title</code> from, for example <code>og:title</code> HTML meta of a <code>webpage</code>. In this case you can provide a fallback scenario:</p>
<div class="highlight highlight-source-python"><pre>title <span class="pl-k">=</span> meta.get(<span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>) <span class="pl-k">or</span> <span class="pl-c1">self</span>._og_search_title(webpage)</pre></div>
<p>This code will try to extract from <code>meta</code> first and if it fails it will try extracting <code>og:title</code> from a <code>webpage</code>.</p>
<h3><a id="user-content-make-regular-expressions-flexible" class="anchor" href="#make-regular-expressions-flexible" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Make regular expressions flexible</h3>
<p>When using regular expressions try to write them fuzzy and flexible.</p>
<h4><a id="user-content-example-2" class="anchor" href="#example-2" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Example</h4>
<p>Say you need to extract <code>title</code> from the following HTML code:</p>
<div class="highlight highlight-text-html-basic"><pre>&lt;<span class="pl-ent">span</span> <span class="pl-e">style</span>=<span class="pl-s"><span class="pl-pds">"</span>position: absolute; left: 910px; width: 90px; float: right; z-index: 9999;<span class="pl-pds">"</span></span> <span class="pl-e">class</span>=<span class="pl-s"><span class="pl-pds">"</span>title<span class="pl-pds">"</span></span>&gt;some fancy title&lt;/<span class="pl-ent">span</span>&gt;</pre></div>
<p>The code for that task should look similar to:</p>
<div class="highlight highlight-source-python"><pre>title <span class="pl-k">=</span> <span class="pl-c1">self</span>._search_regex(
    <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;span<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>class="title"<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">*</span>&gt;(<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&lt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>)<span class="pl-pds">'</span></span>, webpage, <span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>)</pre></div>
<p>Or even better:</p>
<div class="highlight highlight-source-python"><pre>title <span class="pl-k">=</span> <span class="pl-c1">self</span>._search_regex(
    <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;span<span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>class=(<span class="pl-c1">[</span><span class="pl-c1">"</span><span class="pl-cce">\'</span><span class="pl-c1">]</span>)title<span class="pl-ent">\1</span><span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&gt;</span><span class="pl-c1">]</span><span class="pl-k">*</span>&gt;(<span class="pl-ent">?P&lt;title&gt;</span><span class="pl-c1">[</span><span class="pl-k">^</span><span class="pl-c1">&lt;</span><span class="pl-c1">]</span><span class="pl-k">+</span>)<span class="pl-pds">'</span></span>,
    webpage, <span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>, <span class="pl-v">group</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>)</pre></div>
<p>Note how you tolerate potential changes in the <code>style</code> attribute's value or switch from using double quotes to single for <code>class</code> attribute:</p>
<p>The code definitely should not look like:</p>
<div class="highlight highlight-source-python"><pre>title <span class="pl-k">=</span> <span class="pl-c1">self</span>._search_regex(
    <span class="pl-sr"><span class="pl-k">r</span><span class="pl-pds">'</span>&lt;span style="position: absolute; left: 910px; width: 90px; float: right; z-index: 9999;" class="title"&gt;(<span class="pl-c1">.</span><span class="pl-k">*?</span>)&lt;/span&gt;<span class="pl-pds">'</span></span>,
    webpage, <span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>, <span class="pl-v">group</span><span class="pl-k">=</span><span class="pl-s"><span class="pl-pds">'</span>title<span class="pl-pds">'</span></span>)</pre></div>
<h3><a id="user-content-use-safe-conversion-functions" class="anchor" href="#use-safe-conversion-functions" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Use safe conversion functions</h3>
<p>Wrap all extracted numeric data into safe functions from <code>utils</code>: <code>int_or_none</code>, <code>float_or_none</code>. Use them for string to number conversions as well.</p>
<h1><a id="user-content-embedding-youtube-dl" class="anchor" href="#embedding-youtube-dl" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>EMBEDDING YOUTUBE-DL</h1>
<p>youtube-dl makes the best effort to be a good command-line program, and thus should be callable from any programming language. If you encounter any problems parsing its output, feel free to <a href="https://github.com/rg3/youtube-dl/issues/new">create a report</a>.</p>
<p>From a Python program, you can embed youtube-dl in a more powerful fashion, like this:</p>
<div class="highlight highlight-source-python"><pre><span class="pl-k">from</span> <span class="pl-c1">__future__</span> <span class="pl-k">import</span> unicode_literals
<span class="pl-k">import</span> youtube_dl

ydl_opts <span class="pl-k">=</span> {}
<span class="pl-k">with</span> youtube_dl.YoutubeDL(ydl_opts) <span class="pl-k">as</span> ydl:
    ydl.download([<span class="pl-s"><span class="pl-pds">'</span>http://www.youtube.com/watch?v=BaW_jenozKc<span class="pl-pds">'</span></span>])</pre></div>
<p>Most likely, you'll want to use various options. For a list of options available, have a look at <a href="https://github.com/rg3/youtube-dl/blob/master/youtube_dl/YoutubeDL.py#L129-L279"><code>youtube_dl/YoutubeDL.py</code></a>. For a start, if you want to intercept youtube-dl's output, set a <code>logger</code> object.</p>
<p>Here's a more complete example of a program that outputs only errors (and a short message after the download is finished), and downloads/converts the video to an mp3 file:</p>
<div class="highlight highlight-source-python"><pre><span class="pl-k">from</span> <span class="pl-c1">__future__</span> <span class="pl-k">import</span> unicode_literals
<span class="pl-k">import</span> youtube_dl


<span class="pl-k">class</span> <span class="pl-en">MyLogger</span>(<span class="pl-c1">object</span>):
    <span class="pl-k">def</span> <span class="pl-en">debug</span>(<span class="pl-smi"><span class="pl-smi">self</span></span>, <span class="pl-smi">msg</span>):
        <span class="pl-k">pass</span>

    <span class="pl-k">def</span> <span class="pl-en">warning</span>(<span class="pl-smi"><span class="pl-smi">self</span></span>, <span class="pl-smi">msg</span>):
        <span class="pl-k">pass</span>

    <span class="pl-k">def</span> <span class="pl-en">error</span>(<span class="pl-smi"><span class="pl-smi">self</span></span>, <span class="pl-smi">msg</span>):
        <span class="pl-c1">print</span>(msg)


<span class="pl-k">def</span> <span class="pl-en">my_hook</span>(<span class="pl-smi">d</span>):
    <span class="pl-k">if</span> d[<span class="pl-s"><span class="pl-pds">'</span>status<span class="pl-pds">'</span></span>] <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">'</span>finished<span class="pl-pds">'</span></span>:
        <span class="pl-c1">print</span>(<span class="pl-s"><span class="pl-pds">'</span>Done downloading, now converting ...<span class="pl-pds">'</span></span>)


ydl_opts <span class="pl-k">=</span> {
    <span class="pl-s"><span class="pl-pds">'</span>format<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>bestaudio/best<span class="pl-pds">'</span></span>,
    <span class="pl-s"><span class="pl-pds">'</span>postprocessors<span class="pl-pds">'</span></span>: [{
        <span class="pl-s"><span class="pl-pds">'</span>key<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>FFmpegExtractAudio<span class="pl-pds">'</span></span>,
        <span class="pl-s"><span class="pl-pds">'</span>preferredcodec<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>mp3<span class="pl-pds">'</span></span>,
        <span class="pl-s"><span class="pl-pds">'</span>preferredquality<span class="pl-pds">'</span></span>: <span class="pl-s"><span class="pl-pds">'</span>192<span class="pl-pds">'</span></span>,
    }],
    <span class="pl-s"><span class="pl-pds">'</span>logger<span class="pl-pds">'</span></span>: MyLogger(),
    <span class="pl-s"><span class="pl-pds">'</span>progress_hooks<span class="pl-pds">'</span></span>: [my_hook],
}
<span class="pl-k">with</span> youtube_dl.YoutubeDL(ydl_opts) <span class="pl-k">as</span> ydl:
    ydl.download([<span class="pl-s"><span class="pl-pds">'</span>http://www.youtube.com/watch?v=BaW_jenozKc<span class="pl-pds">'</span></span>])</pre></div>
<h1><a id="user-content-bugs" class="anchor" href="#bugs" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>BUGS</h1>
<p>Bugs and suggestions should be reported at: <a href="https://github.com/rg3/youtube-dl/issues">https://github.com/rg3/youtube-dl/issues</a>. Unless you were prompted to or there is another pertinent reason (e.g. GitHub fails to accept the bug report), please do not send bug reports via personal email. For discussions, join us in the IRC channel #youtube-dl on freenode (<a href="http://webchat.freenode.net/?randomnick=1&amp;channels=youtube-dl">webchat</a>).</p>
<p><strong>Please include the full output of youtube-dl when run with <code>-v</code></strong>, i.e. <strong>add</strong> <code>-v</code> flag to <strong>your command line</strong>, copy the <strong>whole</strong> output and post it in the issue body wrapped in ``` for better formatting. It should look similar to this:</p>
<pre><code>$ youtube-dl -v &lt;your command line&gt;
[debug] System config: []
[debug] User config: []
[debug] Command-line args: [u'-v', u'http://www.youtube.com/watch?v=BaW_jenozKcj']
[debug] Encodings: locale cp1251, fs mbcs, out cp866, pref cp1251
[debug] youtube-dl version 2015.12.06
[debug] Git HEAD: 135392e
[debug] Python version 2.6.6 - Windows-2003Server-5.2.3790-SP2
[debug] exe versions: ffmpeg N-75573-g1d0487f, ffprobe N-75573-g1d0487f, rtmpdump 2.4
[debug] Proxy map: {}
...
</code></pre>
<p><strong>Do not post screenshots of verbose logs; only plain text is acceptable.</strong></p>
<p>The output (including the first lines) contains important debugging information. Issues without the full output are often not reproducible and therefore do not get solved in short order, if ever.</p>
<p>Please re-read your issue once again to avoid a couple of common mistakes (you can and should use this as a checklist):</p>
<h3><a id="user-content-is-the-description-of-the-issue-itself-sufficient" class="anchor" href="#is-the-description-of-the-issue-itself-sufficient" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Is the description of the issue itself sufficient?</h3>
<p>We often get issue reports that we cannot really decipher. While in most cases we eventually get the required information after asking back multiple times, this poses an unnecessary drain on our resources. Many contributors, including myself, are also not native speakers, so we may misread some parts.</p>
<p>So please elaborate on what feature you are requesting, or what bug you want to be fixed. Make sure that it's obvious</p>
<ul>
<li>What the problem is</li>
<li>How it could be fixed</li>
<li>How your proposed solution would look like</li>
</ul>
<p>If your report is shorter than two lines, it is almost certainly missing some of these, which makes it hard for us to respond to it. We're often too polite to close the issue outright, but the missing info makes misinterpretation likely. As a committer myself, I often get frustrated by these issues, since the only possible way for me to move forward on them is to ask for clarification over and over.</p>
<p>For bug reports, this means that your report should contain the <em>complete</em> output of youtube-dl when called with the <code>-v</code> flag. The error message you get for (most) bugs even says so, but you would not believe how many of our bug reports do not contain this information.</p>
<p>If your server has multiple IPs or you suspect censorship, adding <code>--call-home</code> may be a good idea to get more diagnostics. If the error is <code>ERROR: Unable to extract ...</code> and you cannot reproduce it from multiple countries, add <code>--dump-pages</code> (warning: this will yield a rather large output, redirect it to the file <code>log.txt</code> by adding <code>&gt;log.txt 2&gt;&amp;1</code> to your command-line) or upload the <code>.dump</code> files you get when you add <code>--write-pages</code> <a href="https://gist.github.com/">somewhere</a>.</p>
<p><strong>Site support requests must contain an example URL</strong>. An example URL is a URL you might want to download, like <code>http://www.youtube.com/watch?v=BaW_jenozKc</code>. There should be an obvious video present. Except under very special circumstances, the main page of a video service (e.g. <code>http://www.youtube.com/</code>) is <em>not</em> an example URL.</p>
<h3><a id="user-content-are-you-using-the-latest-version" class="anchor" href="#are-you-using-the-latest-version" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Are you using the latest version?</h3>
<p>Before reporting any issue, type <code>youtube-dl -U</code>. This should report that you're up-to-date. About 20% of the reports we receive are already fixed, but people are using outdated versions. This goes for feature requests as well.</p>
<h3><a id="user-content-is-the-issue-already-documented" class="anchor" href="#is-the-issue-already-documented" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Is the issue already documented?</h3>
<p>Make sure that someone has not already opened the issue you're trying to open. Search at the top of the window or browse the <a href="https://github.com/rg3/youtube-dl/search?type=Issues">GitHub Issues</a> of this repository. If there is an issue, feel free to write something along the lines of "This affects me as well, with version 2015.01.01. Here is some more information on the issue: ...". While some issues may be old, a new post into them often spurs rapid activity.</p>
<h3><a id="user-content-why-are-existing-options-not-enough" class="anchor" href="#why-are-existing-options-not-enough" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Why are existing options not enough?</h3>
<p>Before requesting a new feature, please have a quick peek at <a href="https://github.com/rg3/youtube-dl/blob/master/README.md#options">the list of supported options</a>. Many feature requests are for features that actually exist already! Please, absolutely do show off your work in the issue report and detail how the existing similar options do <em>not</em> solve your problem.</p>
<h3><a id="user-content-is-there-enough-context-in-your-bug-report" class="anchor" href="#is-there-enough-context-in-your-bug-report" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Is there enough context in your bug report?</h3>
<p>People want to solve problems, and often think they do us a favor by breaking down their larger problems (e.g. wanting to skip already downloaded files) to a specific request (e.g. requesting us to look whether the file exists before downloading the info page). However, what often happens is that they break down the problem into two steps: One simple, and one impossible (or extremely complicated one).</p>
<p>We are then presented with a very complicated request when the original problem could be solved far easier, e.g. by recording the downloaded video IDs in a separate file. To avoid this, you must include the greater context where it is non-obvious. In particular, every feature request that does not consist of adding support for a new site should contain a use case scenario that explains in what situation the missing feature would be useful.</p>
<h3><a id="user-content-does-the-issue-involve-one-problem-and-one-problem-only" class="anchor" href="#does-the-issue-involve-one-problem-and-one-problem-only" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Does the issue involve one problem, and one problem only?</h3>
<p>Some of our users seem to think there is a limit of issues they can or should open. There is no limit of issues they can or should open. While it may seem appealing to be able to dump all your issues into one ticket, that means that someone who solves one of your issues cannot mark the issue as closed. Typically, reporting a bunch of issues leads to the ticket lingering since nobody wants to attack that behemoth, until someone mercifully splits the issue into multiple ones.</p>
<p>In particular, every site support request issue should only pertain to services at one site (generally under a common domain, but always using the same backend technology). Do not request support for vimeo user videos, White house podcasts, and Google Plus pages in the same issue. Also, make sure that you don't post bug reports alongside feature requests. As a rule of thumb, a feature request does not include outputs of youtube-dl that are not immediately related to the feature at hand. Do not post reports of a network error alongside the request for a new video service.</p>
<h3><a id="user-content-is-anyone-going-to-need-the-feature" class="anchor" href="#is-anyone-going-to-need-the-feature" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Is anyone going to need the feature?</h3>
<p>Only post features that you (or an incapacitated friend you can personally talk to) require. Do not post features because they seem like a good idea. If they are really useful, they will be requested by someone who requires them.</p>
<h3><a id="user-content-is-your-question-about-youtube-dl" class="anchor" href="#is-your-question-about-youtube-dl" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Is your question about youtube-dl?</h3>
<p>It may sound strange, but some bug reports we receive are completely unrelated to youtube-dl and relate to a different, or even the reporter's own, application. Please make sure that you are actually using youtube-dl. If you are using a UI for youtube-dl, report the bug to the maintainer of the actual application providing the UI. On the other hand, if your UI for youtube-dl fails in some way you believe is related to youtube-dl, by all means, go ahead and report the bug.</p>
<h1><a id="user-content-copyright" class="anchor" href="#copyright" aria-hidden="true"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>COPYRIGHT</h1>
<p>youtube-dl is released into the public domain by the copyright holders.</p>
<p>This README file was originally written by <a href="https://github.com/dbbolton">Daniel Bolton</a> and is likewise released into the public domain.</p>
</article>
  </div>

  </div>

  <button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
  <div id="jump-to-line" style="display:none">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
      <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
      <button type="submit" class="btn">Go</button>
</form>  </div>






  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>



    </div>
  </div>

  </div>

      
<div class="container site-footer-container">
  <div class="site-footer " role="contentinfo">
    <ul class="site-footer-links float-right">
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact GitHub</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage" class="site-footer-mark" title="GitHub">
      <svg aria-hidden="true" class="octicon octicon-mark-github" height="24" version="1.1" viewBox="0 0 16 16" width="24"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2017 <span title="0.12271s from unicorn-168610123-5p9rh">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error">
    <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"/></svg>
    <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
    </button>
    You can't perform that action at this time.
  </div>


    <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/compat-8a4318ffea09a0cdb8214b76cf2926b9f6a0ced318a317bed419db19214c690d.js"></script>
    <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-73720f027bb317fceb118c259275da4be5efa344c246a12341a68c3168ceeaa7.js"></script>
    <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-18dfc890c7a4a84c1427f5c55cb238d1280a2136917379c4eeba395ae950686f.js"></script>
    
    
    
    
  <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
    <svg aria-hidden="true" class="octicon octicon-alert" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M8.865 1.52c-.18-.31-.51-.5-.87-.5s-.69.19-.87.5L.275 13.5c-.18.31-.18.69 0 1 .19.31.52.5.87.5h13.7c.36 0 .69-.19.86-.5.17-.31.18-.69.01-1L8.865 1.52zM8.995 13h-2v-2h2v2zm0-3h-2V6h2v4z"/></svg>
    <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg aria-hidden="true" class="octicon octicon-x" height="16" version="1.1" viewBox="0 0 12 16" width="12"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48z"/></svg>
    </button>
  </div>
</div>


  </body>
</html>

