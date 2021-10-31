### PSR-5:PHPDoc
## Introduction
-**Describe** a standard for implementing annotations via PHPDoc. Although it does offer versatility which makes it possible to create a subsequent PSR based on current practices. See chapter 5.3 for more information on this topic.
-**Describe best** practices or recommendations for Coding Standards on the application of the PHPDoc standard. This document is limited to a formal specification of syntax and intention
Definitions [Link](https://github.com/php-fig/fig-standards/blob/master/proposed/phpdoc.md)
```
/**
 * This class acts as an example on where to position a DocBlock.
 */
class Foo
{
    /** @var string|null $title contains a title for the Foo */
    protected $title = null;

    /**
     * Sets a single-line title.
     *
     * @param string $title A text for the title.
     *
     * @return void
     */
    public function setTitle($title)
    {
        // there should be no docblock here
        $this->title = $title;
    }
}
```

Number | Name | Keyword
--- | --- | ---
*1* | *name* | 123456
