Download Link: https://assignmentchef.com/product/solved-assignment-04-searching-sorting-and-algorithm-analysis
<br>
<h2><a id="user-content-requirements" class="anchor" href="https://github.com/timferido/assignment-04#requirements" aria-hidden="true"></a>Requirements</h2>

You are allowed to write everything in one file this time, so long it is organized and the file is not too long. If the file gets too long, please split it into multiple <code>.h</code> and <code>.cpp</code> files, and have a <code>main.cpp</code> that <code>#include</code>s the <code>.h</code> files, and can be used to call the functions prototyped in them.

All the files you produce must be able to exist within a single project. You will submit these files via github as normal.

<h3><a id="user-content-setup" class="anchor" href="https://github.com/timferido/assignment-04#setup" aria-hidden="true"></a>Setup</h3>

<ul>

 <li>Write a function named <code>print_vector</code> that takes a <code>const std::vector&lt;int&gt; &amp;</code> as an argument, and outputs the contents (separated by whitespace) to stdout (followed by a newline).</li>

 <li>Write the <code>main</code> function. It doesn’t need to do anything right now, but as you write the functions below, you should put code in <code>main</code> to test them.</li>

</ul>

<h3><a id="user-content-selection-sort" class="anchor" href="https://github.com/timferido/assignment-04#selection-sort" aria-hidden="true"></a>Selection Sort</h3>

Write a function named <code>selection_sort</code> that takes a <code>std::vector&lt;int&gt; &amp;</code> as an argument, and sorts it in-place. The algorithm is as follows:

<ol start="0">

 <li>For the index of each element in the array (the “current index”)</li>

 <li>Find the index of the minimum element at or after the current index.</li>

 <li>Swap the element at the current index with the smallest element found.</li>

</ol>

For a more thorough explanation, google around, or see <a href="https://en.wikipedia.org/wiki/Selection_sort" rel="nofollow">the relevant Wikipedia entry</a>.

<h3><a id="user-content-merge-sort" class="anchor" href="https://github.com/timferido/assignment-04#merge-sort" aria-hidden="true"></a>Merge Sort</h3>

Write a function named <code>merge_sort</code> that takes as an argument a <code>const std::vector&lt;int&gt; &amp;</code> and returns a <code>std::vector&lt;int&gt;</code>containing all the elements of the vector that was passed as an argument, in ascending order. The algorithm (which is recursive) is as follows:

<ol start="0">

 <li>If the vector contains only 1 element, return the vector unchanged.</li>

 <li>Otherwise, split the vector into two halves, named <code>left</code> and <code>right</code>.</li>

 <li>Recursively sort each half (i.e. call <code>merge_sort(left);</code> and <code>merge_sort(right);</code>).</li>

 <li>Merge <code>left</code> and <code>right</code> into a new vector named <code>sorted</code>, in the following manner:

  <ol start="0">

   <li>As long as <code>left</code> and <code>right</code> both have elements not in <code>sorted</code>, compare the smallest such elements of each list, take the smaller of the two, and append it to <code>sorted</code>.</li>

   <li>Once all of the elements of either <code>left</code> or <code>right</code> are in <code>sorted</code>, take the leftover elements and append them to <code>sorted</code>.</li>

  </ol></li>

 <li>Return <code>sorted</code>.</li>

</ol>

For a more thorough explanation, google around, or see <a href="https://en.wikipedia.org/wiki/Merge_sort" rel="nofollow">the relevant Wikipedia entry</a>.

You may need to search around for the best way to split a vector into two smaller vectors. Here’s <a href="https://stackoverflow.com/a/9811343" rel="nofollow">one way</a> from stackoverflow.

<h2><a id="user-content-requests" class="anchor" href="https://github.com/timferido/assignment-04#requests" aria-hidden="true"></a>Requests</h2>

<ul>

 <li>Please try to do this in groups, and try to use Google, etc., only for answers to questions about the language (as opposed to questions about this problem).</li>

</ul>

<h2><a id="user-content-assumptions" class="anchor" href="https://github.com/timferido/assignment-04#assumptions" aria-hidden="true"></a>Assumptions</h2>

(None)

<h2><a id="user-content-style" class="anchor" href="https://github.com/timferido/assignment-04#style" aria-hidden="true"></a>Style</h2>

<ul>

 <li>Place your solution in a <code>solution--YOURNAME</code> subdirectory (where <code>YOURNAME</code> is your GitHub username).</li>

 <li>Include your copyright and license information at the top of every file, followed by a brief description of the file’s contents, e.g.</li>

 <li>Use “include guards” in all <code>.h</code> files. Be sure to give the preprocessor variable a name corresponding to the file name. For example, in <code>point.h</code>:</li>

 <li><code>main()</code> must have its own <code>.cpp</code> file. I suggest calling it <code>main.cpp</code>.</li>

 <li>Classes must have both <code>.h</code> and <code>.cpp</code> files, with member functions defined in the <code>.cpp</code> files unless they are truly trivial. If it makes sense, you may put multiple classes into one pair of <code>.h</code> and <code>.cpp</code> files.</li>

 <li>Declare member functions and function arguments as <code>const</code> when appropriate (in general, whenever possible).</li>

 <li>Document and format your code well and consistently. Be sure to clearly document the source of any code, algorithm, information, etc. that you use or reference while completing your work.</li>

 <li>Wrap lines at 79 or 80 columns whenever possible.</li>

 <li>End your file with a blank line.</li>

 <li>Do <em>not</em> use <code>using namespace std;</code>. You may get around typing <code>std::</code> in front of things or with, e.g., <code>using std::cout;</code>.</li>

</ul>

5/5 - (1 vote)

<pre><span class="pl-c">/* ----------------------------------------------------------------------------</span><span class="pl-c"> * Copyright &amp;copy; 2016 Ben Blazak &lt;<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5331313f322932381335263f3f3621273c3d7d363726">[email protected]</a>&gt;</span><span class="pl-c"> * Released under the [MIT License] (http://opensource.org/licenses/MIT)</span><span class="pl-c"> * ------------------------------------------------------------------------- */</span><span class="pl-c">/**</span><span class="pl-c"> * A short program to print "Hello World!" to standard output.</span><span class="pl-c"> */</span></pre>