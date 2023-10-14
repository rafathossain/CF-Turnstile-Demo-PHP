<h1>Cloudflare Turnstile Demo with PHP</h1>

<p>This repository contains a simple demonstration of how to integrate Cloudflare Turnstile into your PHP-based web application. Turnstile is a security feature provided by Cloudflare that allows you to implement various challenges to protect your site from malicious traffic.</p>

<h2>Prerequisites</h2>
<p>Before you can run this demo, make sure you have the following prerequisites:</p>
<ul>
    <li>PHP installed on your web server.</li>
    <li>A Cloudflare account.</li>
    <li>A Cloudflare site key and secret key.</li>
</ul>

<h2>Configuration</h2>
<p>In the PHP code, you'll need to set your Cloudflare site key and secret key as follows:</p>
<code>
    $CF_SITE_KEY = "1x00000000000000000000AA";
    $CF_SECRET_KEY = "1x0000000000000000000000000000000AA";
</code>
<p>You should replace the above placeholder keys with your actual Cloudflare site key and secret key.</p>

<h2>Dummy Site Keys and Secret Keys</h2>
<p>For testing purposes, we provide the following dummy site keys and secret keys. These keys can be used in your development environment to test the Turnstile challenges without affecting your production environment.</p>

<h2>Dummy Site Keys and Secret Keys</h2>
<p>For testing purposes, we provide the following dummy site keys and secret keys. These keys can be used in your development environment to test the Turnstile challenges without affecting your production environment.</p>

<table>
    <tr>
        <th>Sitekey</th>
        <th>Description</th>
        <th>Visibility</th>
    </tr>
    <tr>
        <td>1x00000000000000000000AA</td>
        <td>Always passes</td>
        <td>Visible</td>
    </tr>
    <tr>
        <td>2x00000000000000000000AB</td>
        <td>Always blocks</td>
        <td>Visible</td>
    </tr>
    <tr>
        <td>1x00000000000000000000BB</td>
        <td>Always passes</td>
        <td>Invisible</td>
    </tr>
    <tr>
        <td>2x00000000000000000000BB</td>
        <td>Always blocks</td>
        <td>Invisible</td>
    </tr>
    <tr>
        <td>3x00000000000000000000FF</td>
        <td>Forces an interactive challenge</td>
        <td>Visible</td>
    </tr>
</table>

<p><strong>Secret Keys</strong></p>
<ul>
    <li>Secret key: <code>1x0000000000000000000000000000000AA</code> - Always passes</li>
    <li>Secret key: <code>2x0000000000000000000000000000000AA</code> - Always fails</li>
    <li>Secret key: <code>3x0000000000000000000000000000000AA</code> - Yields a "token already spent" error</li>
</ul>

<h2>Usage</h2>
<ol>
    <li>Clone this repository to your local development environment or web server.</li>
    <li>Configure the Cloudflare site key and secret key in the PHP file, as mentioned in the "Configuration" section.</li>
    <li>Run the PHP script on your server.</li>
</ol>

<h2>Important Notes</h2>
<p>Do not use the dummy site keys and secret keys in your production environment. These keys are meant for testing and development only.</p>
<p>Ensure that you have Cloudflare properly set up with Turnstile in your production environment for real security protection.</p>

<h2>License</h2>
<p>This project is licensed under the MIT License - see the <a href="LICENSE">LICENSE</a> file for details.</p>

<p>For more information on Cloudflare and Turnstile, visit the <a href="https://developers.cloudflare.com/turnstile">Cloudflare documentation</a>.</p>

<p>Feel free to report any issues or provide feedback in the <a href="https://github.com/your-repo/issues">Issues</a> section of this repository.</p>

<p>Happy coding!</p>