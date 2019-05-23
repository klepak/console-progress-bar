# Console Progress Bar
Outputs a progress bar to console.

## Example
```php
$progress = (new ConsoleProgressBar)
            ->max(5)
            ->message('Test')
            ->unit('Things')
            ->padding(1, 2); # top, bottom

sleep(1);

$progress->update(3);

sleep(1);

$progress->completed();
```