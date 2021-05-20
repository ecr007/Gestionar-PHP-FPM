# Gestionar-PHP-FPM

<div class="post_content">
<div style="float: right; margin-top: 0; margin-left: 5px;"><a title="See all PHP related FAQ" href="//www.cyberciti.biz/faq/category/php/"><noscript><img src="https://www.cyberciti.biz/media/new/category/old/php-logo.png" alt="" border="0" /></noscript><img class=" lazyloaded" src="https://www.cyberciti.biz/media/new/category/old/php-logo.png" data-src="https://www.cyberciti.biz/media/new/category/old/php-logo.png" alt="" border="0"></a></div><span class="drop_cap">I</span> am a new Linux and Unix system user. I want to reload or restart my PHP-fpm service. How do I restart PHP-fpm? How do you restart php7.0-fpm on Ubuntu Linux 16.04 LTS server?<br>
<span id="more-146069"></span><br>
PHP-FPM is nothing but a straightforward and robust FastCGI Process Manager for PHP. You can use it with Apache, Nginx, and other web servers. It includes many advanced features. Let us see how to stop or restart or reload PHP-FPM after you update php.ini file. <center>
<ins class="adsbygoogle tips_inline_slot_1" data-ad-client="ca-pub-7825705102693166" data-ad-slot="7261197400"><iframe id="aswift_2" style="height: 1px !important; max-height: 1px !important; max-width: 1px !important; width: 1px !important;"><iframe id="google_ads_frame1"></iframe></iframe></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>
</center>
<p></p>
<noscript><img src="https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001.jpeg" alt="How do you restart php-fpm?" width="599" height="449" class="aligncenter size-full wp-image-146070" srcset="https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001.jpeg 599w, https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001-300x225.jpeg 300w" sizes="(max-width: 599px) 100vw, 599px" /></noscript><img src="https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001.jpeg" data-src="https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001.jpeg" alt="How do you restart php-fpm?" width="599" height="449" class="aligncenter size-full wp-image-146070 lazyloaded" data-srcset="https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001.jpeg 599w, https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001-300x225.jpeg 300w" data-sizes="(max-width: 599px) 100vw, 599px" sizes="(max-width: 599px) 100vw, 599px" srcset="https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001.jpeg 599w, https://www.cyberciti.biz/media/new/faq/2017/04/welcome-php-fpm-restart-reload-linux-unix-command.001-300x225.jpeg 300w">
<h2>How do I edit php.ini or www.conf file?</h2>
<p>To edit php.ini type:<br>
<code>$ sudo vi /etc/php5/php.ini </code><br>
OR<br>
<code>$ sudo vi /etc/php/7.0/fpm/php.ini</code><br>
To edit php-fpm config file:<br>
<code>$ sudo vi /etc/php/7.0/fpm/php-fpm.conf<br>
$ sudo vi /etc/php/7.0/fpm/pool.d/www.conf</code><br>
Once edited, save and close the file. Now you need to run command as per your Linux/Unix distro version after editing the file.</p>
<h2>Start php-fpm on <span style="color: rgb(153, 102, 51);">CentOS/RHEL 7</span></h2>
<p><code>$ sudo systemctl start php-fpm</code></p>
<h2>Stop php-fpm <span style="color: rgb(153, 102, 51);">CentOS/RHEL 7</span></h2>
<p><code>$ sudo systemctl stop php-fpm</code></p>
<h2>Reload php-fpm <span style="color: rgb(153, 102, 51);">CentOS/RHEL 7</span></h2>
<p><code>$ sudo systemctl reload php-fpm</code></p>
<h2>Restart php-fpm <span style="color: rgb(153, 102, 51);">CentOS/RHEL 7</span></h2>
<p><code>$ sudo systemctl restart php-fpm</code></p>
<h2>Start/stop/restart/reload php-fpm on <span style="color: rgb(255, 153, 0);">CentOS/RHEL 6.x or older</span></h2>
<p>Type the following command:<br>
<code>$ sudo service php-fpm start <span style="color: rgb(0, 153, 0);"># &lt;- start it</span><br>
$ sudo service php-fpm stop <span style="color: rgb(0, 153, 0);"># &lt;- stop it</span><br>
$ sudo service php-fpm restart <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span><br>
$ sudo service php-fpm reload <span style="color: rgb(0, 153, 0);"># &lt;- reload it</span></code></p>
<h2>How to start/stop/restart/reload <span style="color: rgb(102, 51, 51);">php5-fpm (php version 5.x)</span> on Ubuntu/Debian Linux</h2>
<p><code>$ sudo service php5-fpm start<br>
$ sudo service php5-fpm stop<br>
$ sudo service php5-fpm restart <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span><br>
$ sudo service php5-fpm reload <span style="color: rgb(0, 153, 0);"># &lt;- reload it</span></code><br>
OR if you are using systemd based distro such as Ubuntu Linux 16.04+ LTS or Debian Linux 8.x+:<br>
<code>$ sudo systemctl start php7.0-fpm.service<br>
$ sudo systemctl stop php5-fpm.service<br>
$ sudo systemctl restart php5-fpm.service <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span><br>
$ sudo systemctl reload php5-fpm.service <span style="color: rgb(0, 153, 0);"># &lt;- reload it</span></code></p>
<h2>How to start/stop/restart/reload <span style="color: rgb(0, 153, 0);">php7.0-fpm (php version 7.x)</span> on Ubuntu/Debian Linux </h2>
<p><code>$ sudo service php7.0-fpmstart<br>
$ sudo service php7.0-fpm stop<br>
$ sudo service php7.0-fpm restart <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span><br>
$ sudo service php7.0-fpm reload <span style="color: rgb(0, 153, 0);"># &lt;- reload it</span></code><br>
OR if you are using systemd based distro such as Ubuntu Linux 16.04+ LTS or Debian Linux 8.x+:<br>
<code>$ sudo systemctl start php7.0-fpm.service<br>
$ sudo systemctl stop php7.0-fpm.service<br>
$ sudo systemctl restart php7.0-fpm.service <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span><br>
$ sudo systemctl reload php7.0-fpm.service <span style="color: rgb(0, 153, 0);"># &lt;- reload it</span></code></p>
<h2>How do you restart/reload php-fpm on <span style="color: rgb(102, 102, 204);">Alpine Linux</span>?</h2>
<p>The syntax is:<br>
<code># /etc/init.d/php-fpm start<br>
# /etc/init.d/php-fpm stop<br>
# /etc/init.d/php-fpm restart <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span></code></p>
<h2>How do you restart/reload php-fpm on <span style="color: rgb(153, 51, 153);">FreeBSD unix</span>?</h2>
<p>The syntax is<br>
<code># /usr/local/etc/rc.d/php-fpm start<br>
# /usr/local/etc/rc.d/php-fpm stop<br>
# /usr/local/etc/rc.d/php-fpm reload <span style="color: rgb(0, 153, 0);"># &lt;- reload it</span><br>
# /usr/local/etc/rc.d/php-fpm restart <span style="color: rgb(0, 153, 0);"># &lt;- restart it</span></code><br>
OR use the service command:<br>
<code># service php-fpm start<br>
# service php-fpm stop<br>
# service php-fpm restart<br>
# service php-fpm reload</code></p>
<br>


<br>
 </div>
