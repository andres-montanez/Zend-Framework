Add on your deps

<pre><code>[ZendFramework]
    git=http://github.com/andres-montanez/Zend-Framework.git
    version=v1.11.11
    target=/zend-framework
</code></pre>

And then
```
  bin/vendors install
```

And last, register the prefix on autoload.php
<pre><code>$loader->registerPrefixes(array(
    ...
    'Zend_' => __DIR__.'/../vendor/zend-framework',
));
</code></pre>
