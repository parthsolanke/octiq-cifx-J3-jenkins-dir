# CI detection fixture

`dir('backend') { sh 'npm test' }`. ONLY backend/package.json has a test script - the root deliberately has none, so a dir() that is not resolved produces a visibly different verdict.

Expected verdict line in the Octiq chat:

    Tests required - CI runs `npm test`   (cwd backend)
