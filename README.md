# stream-merge-sort

Merge (interleave) a bunch of ordered streams and keep the order.

[![build status](https://secure.travis-ci.org/grncdr/merge-stream.svg?branch=master)](http://travis-ci.org/grncdr/merge-stream)

## Synopsis

```javascript
var stream1 = new Stream();
var stream2 = new Stream();

var mergedSorted = mergeStreamsSort([stream1, stream2], function(a, b) { return a.id < b.id });
```

## Description

This is the merge function from [event-stream](https://github.com/dominictarr/event-stream) separated into a new module and given an `add` method so you can dynamically add more sources to the stream.

## License

MIT