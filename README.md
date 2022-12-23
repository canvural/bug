## Steps to reproduce

```console
git clone https://github.com/canvural/bug.git
cd bug
composer install
./vendor/bin/phpunit
```

See that `FooTest` fails.

To prove the other way, change `checkFoo` to true in `extension.neon` and rerun the tests. Now `FooTest` passes but `BarTest` fails.