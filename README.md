This is a live demo for the issue with setting class in custom element constructor.
This looks to be broken in certain cases, but I'm not quite sure where exactly and how it should behave.

For example, Safari fails in two tests, but it seems like this is indeed the right behavior and it must fail. But it does not fail in others where it must fail too. Chrome only fails in one and must fail in others as well. Firefox ignores the problem and works without any issues, may be due to the implementation of the polyfill for custom elements.

```sh
bower install
polymer serve
# open tests in different browsers
# http://127.0.0.1:8081/components/bug-custom-element-set-class-in-constructor/test/
```
