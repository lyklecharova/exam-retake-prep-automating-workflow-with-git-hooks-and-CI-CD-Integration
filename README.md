<h1>pre-commit</h1>

<p>
#!/bin/sh

echo "🖌️ Checking code format with Prettier..."
npx prettier --check .

if [ $? -ne 0 ]; then
echo "❌ Code is not formatted correctly. Commit aborted."
exit 1
fi

echo "✅ Code is formatted. Proceeding with commit."

</p>
<br/>
<h1>pre-push</h1>

<p>
#!/bin/sh

echo "🧪 Running tests before push..."
npm test

if [ $? -ne 0 ]; then
echo "❌ Tests failed. Push aborted."
exit 1
fi

echo "✅ Tests passed. Proceeding with push"

</p>
 <br/>
<ul>
<p> This is a git log graph all</p>
<img src= "./{5A600DF6-72A4-41E8-BB56-1B9086D477E6}.png" alt="Git log --graph --all"/>
</ul>
<br/>
 
<ul>
<p> This is a git reflog</p>
<img src= "./{5A600DF6-72A4-41E8-BB56-1B9086D477E6}.png" alt="Git reflog"/>
</ul>
<br/>
