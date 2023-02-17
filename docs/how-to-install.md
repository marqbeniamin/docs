---
sidebar_position: 2
title: How to install
---
import BrowserOnly from '@docusaurus/BrowserOnly';

export const CurrentSite = () => {
  return (
    <BrowserOnly>
      {() =>  new URLSearchParams(window.location.search).get('site') || 'exapmle.com'}
    </BrowserOnly>
  );
};

export const GetScript = () => {
  return (
    <BrowserOnly>
      {() => {
        const current_site = new URLSearchParams(window.location.search).get('site') || 'exapmle.com';
        return <code>{`<script src="https://nepcha.com/install.js" data-domain="${current_site}"></script>`}</code>;
      }}
    </BrowserOnly>
  );
};




<h2> Install Nepcha on your site (<CurrentSite/>)</h2>

1. Add the following script to your site:

<GetScript/>
