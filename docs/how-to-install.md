---
sidebar_position: 2
title: How to install
---

export const current_site = new URLSearchParams(window.location.search).get('site') || 'exapmle.com';

<!-- code with script -->
export const GetScript = () => (
  <pre>
    <code>
      {`<script src="https://nepcha.com/script.js" data-domain="${current_site}"></script>`}
    </code>
  </pre>
);




<h2> Install Nepcha on your site ({current_site})</h2>

1. Add the following script to your site:

export const current_script = "text"

<GetScript></GetScript>
