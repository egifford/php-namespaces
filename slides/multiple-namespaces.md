### Multiple namespaces

<pre class="fragment-replacement"><code class="hljs lang-php fragment fade-out" data-fragment-index="0">&lt;?php

namespace My\Project;

function doSomething() {/* ... */}</code><span class="fragment fade-out" data-fragment-index="1"><code class="hljs lang-php fragment fade-in" data-fragment-index="0">&lt;?php

namespace My\Project;

function doSomething() {/* ... */}

namespace My\Project\Services;

function doSomethingElse() {/* ... */}</code></span><code class="hljs lang-php fragment fade-in" data-fragment-index="1">&lt;?php

namespace My\Project {
    function doSomething() {/* ... */}
}

namespace My\Project\Services {
    function doSomethingElse() {/* ... */}
}</code></pre>

Note:

You can also _technically_ define multiple namespaces in the same file, though I've never seen this done in production.

Can even wrap them in brackets for readability, but YUCK!
