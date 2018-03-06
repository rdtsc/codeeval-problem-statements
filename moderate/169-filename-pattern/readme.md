<h2>Filename Pattern</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a filename pattern and a list of filenames. Find out which filenames from the list are matching the
    given pattern. The pattern can contain characters and the following wildcards:
</p>

<ul>
<li>? &#x2014; matches any single character.</li>
<li>* &#x2014; matches everything (any multiple characters, any single character, or empty string).</li>
<li>[abc] &#x2014; matches any character inside brackets (in this example: a, b, or c).</li>
</ul>

<p>
    Matching is case-sensitive.
</p>

<h3>Input sample:</h3>

<p>
    The first argument is a file that contains space-separated filename pattern and filenames.
</p>
<p>
    For example:
</p>

<pre class="description-input-output">*7* johab.py gen_probe.ko palmtx.h macpath.py tzp dm-dirty-log.h bh1770.h pktloc faillog.8.gz zconf.gperf
*[0123456789]*[auoei]* IBM1008_420.so zfgrep limits.conf.5.gz tc.h ilogb.3.gz limits.conf CyrAsia-TerminusBold28x14.psf.gz nf_conntrack_sip.ko DistUpgradeViewNonInteractive.pyc NFKDQC
*.??? max_user_watches arptables.h net_namespace Kannada.pl menu_no_no.utf-8.vim shtags.1 unistd_32_ia32.h gettext-tools.mo ntpdate.md5sums linkat.2.gz
*.pdf OldItali.pl term.log plymouth-upstart-bridge rand.so libipw.ko jisfreq.pyc impedance-analyzer xmon.h 1.5.0.3.txt bank
g*.* 56b8a0b6.0 sl.vim digctl.h groff-base.conffiles python-software-properties.md5sums CountryInformation.py use_zero_page session-noninteractive d2i_RSAPublicKey.3ssl.gz container-detect.log.4.gz
*[0123456789]* keyboard.h machinecheck 46b2fd3b.0 libip6t_frag.so timer_defs.h nano-menu.xpm NI vim-keys.conf setjmp.h memcg</pre>

<h3>Output sample:</h3>

<p>
    Print filenames matching a given pattern to stdout. If there are no such files, print a minus &#x2018;-&#x2019; character.
</p>
<p>
    For example:
</p>
<pre class="description-input-output">bh1770.h
IBM1008_420.so
menu_no_no.utf-8.vim
-
groff-base.conffiles
46b2fd3b.0 libip6t_frag.so</pre>

<h3>Constraints:</h3>
<ol>
<li>Matching is case-sensitive.</li>
<li>Filenames cannot contain spaces.</li>
<li>There are 40 test cases and 100 filenames in every test case.</li>
</ol>