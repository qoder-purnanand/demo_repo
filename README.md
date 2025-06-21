<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Git Commands Documentation</title>
</head>

<h1>Git Commands Documentation</h1>

<p>This document contains a collection of commonly used <code>git</code> commands, categorized and explained for easy reference.</p>

<hr>

<h2><strong>Basic Git Commands</strong></h2>

<ul>
    <li><strong>1. <code>git init</code></strong>
        <p><strong>Description</strong>: Initializes a new Git repository.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git init</code></pre>
    </li>
    <li><strong>2. <code>git clone</code></strong>
        <p><strong>Description</strong>: Clones an existing repository into a new directory.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git clone &lt;repository_url&gt;</code></pre>
    </li>
    <li><strong>3. <code>git status</code></strong>
        <p><strong>Description</strong>: Displays the state of the working directory and staging area.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git status</code></pre>
    </li>
    <li><strong>4. <code>git add</code></strong>
        <p><strong>Description</strong>: Stages changes (add files to the staging area).</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git add &lt;file_name&gt;</code></pre>
        <pre><code>git add .</code></pre>
    </li>
    <li><strong>5. <code>git commit</code></strong>
        <p><strong>Description</strong>: Commits the staged changes to the repository.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git commit -m "Commit message"</code></pre>
    </li>
    <li><strong>6. <code>git push</code></strong>
        <p><strong>Description</strong>: Pushes local commits to a remote repository.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git push origin &lt;branch_name&gt;</code></pre>
    </li>
    <li><strong>7. <code>git pull</code></strong>
        <p><strong>Description</strong>: Fetches and merges changes from the remote repository into the current branch.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git pull origin &lt;branch_name&gt;</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Branching Commands</strong></h2>

<ul>
    <li><strong>1. <code>git branch</code></strong>
        <p><strong>Description</strong>: Lists all local branches, or creates a new branch.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git branch</code></pre>
        <pre><code>git branch &lt;branch_name&gt;</code></pre>
    </li>
    <li><strong>2. <code>git checkout</code></strong>
        <p><strong>Description</strong>: Switches to a different branch or commit.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git checkout &lt;branch_name&gt;</code></pre>
        <pre><code>git checkout -b &lt;branch_name&gt;</code></pre>
    </li>
    <li><strong>3. <code>git merge</code></strong>
        <p><strong>Description</strong>: Merges changes from another branch into the current branch.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git merge &lt;branch_name&gt;</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Remote Commands</strong></h2>

<ul>
    <li><strong>1. <code>git remote</code></strong>
        <p><strong>Description</strong>: Manages remote repositories.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git remote add &lt;name&gt; &lt;url&gt;</code></pre>
        <pre><code>git remote remove &lt;name&gt;</code></pre>
        <pre><code>git remote -v</code></pre>
    </li>
    <li><strong>2. <code>git fetch</code></strong>
        <p><strong>Description</strong>: Fetches changes from the remote repository but doesn't merge them.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git fetch origin</code></pre>
    </li>
    <li><strong>3. <code>git push --force</code></strong>
        <p><strong>Description</strong>: Forcefully pushes changes to a remote repository (use with caution).</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git push --force origin &lt;branch_name&gt;</code></pre>
    </li>
</ul>

<hr>

<h2><strong>History & Log Commands</strong></h2>

<ul>
    <li><strong>1. <code>git log</code></strong>
        <p><strong>Description</strong>: Shows the commit history.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git log</code></pre>
        <pre><code>git log --oneline</code></pre>
    </li>
    <li><strong>2. <code>git diff</code></strong>
        <p><strong>Description</strong>: Shows the differences between changes.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git diff</code></pre>
        <pre><code>git diff &lt;commit&gt;</code></pre>
    </li>
    <li><strong>3. <code>git revert</code></strong>
        <p><strong>Description</strong>: Reverts a specific commit (creates a new commit to undo changes).</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git revert &lt;commit_hash&gt;</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Advanced Commands</strong></h2>

<ul>
    <li><strong>1. <code>git reset</code></strong>
        <p><strong>Description</strong>: Resets the current branch to a specific commit.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git reset --hard &lt;commit_hash&gt;</code></pre>
        <pre><code>git reset &lt;commit_hash&gt;</code></pre>
    </li>
    <li><strong>2. <code>git rebase</code></strong>
        <p><strong>Description</strong>: Re-applies commits on top of another base commit.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git rebase &lt;branch_name&gt;</code></pre>
    </li>
    <li><strong>3. <code>git stash</code></strong>
        <p><strong>Description</strong>: Stashes changes in the working directory to apply later.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git stash</code></pre>
        <pre><code>git stash apply</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Tagging Commands</strong></h2>

<ul>
    <li><strong>1. <code>git tag</code></strong>
        <p><strong>Description</strong>: Adds a tag to a specific commit.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git tag &lt;tag_name&gt;</code></pre>
        <pre><code>git tag -a &lt;tag_name&gt; -m "Message"</code></pre>
        <pre><code>git tag &lt;tag_name&gt; &lt;commit_hash&gt;</code></pre>
    </li>
    <li><strong>2. <code>git push --tags</code></strong>
        <p><strong>Description</strong>: Pushes all tags to the remote repository.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git push --tags</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Configuration Commands</strong></h2>

<ul>
    <li><strong>1. <code>git config</code></strong>
        <p><strong>Description</strong>: Configures Git settings (user name, email, etc.).</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git config --global user.name "Your Name"</code></pre>
        <pre><code>git config --global user.email "you@example.com"</code></pre>
        <pre><code>git config --list</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Undoing Changes</strong></h2>

<ul>
    <li><strong>1. <code>git checkout -- &lt;file&gt;</code></strong>
        <p><strong>Description</strong>: Discards changes in a file (reverts to the last commit).</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git checkout -- &lt;file_name&gt;</code></pre>
    </li>
    <li><strong>2. <code>git reset &lt;file&gt;</code></strong>
        <p><strong>Description</strong>: Unstages a file but keeps the changes in the working directory.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git reset &lt;file_name&gt;</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Miscellaneous Commands</strong></h2>

<ul>
    <li><strong>1. <code>git rm</code></strong>
        <p><strong>Description</strong>: Removes a file from both the working directory and staging area.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git rm &lt;file_name&gt;</code></pre>
    </li>
    <li><strong>2. <code>git mv</code></strong>
        <p><strong>Description</strong>: Moves or renames a file.</p>
        <p><strong>Usage</strong>:</p>
        <pre><code>git mv &lt;old_file_name&gt; &lt;new_file_name&gt;</code></pre>
    </li>
</ul>

<hr>

<h2><strong>Conclusion</strong></h2>

<p>This document includes only the basic and frequently used <code>git</code> commands. For more advanced features, you can refer to the official Git documentation at <a href="https://git-scm.com/doc" target="_blank">https://git-scm.com/doc</a>.</p>

</html>
