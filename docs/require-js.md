# Implementing 3q.js with require.js

For using 3q.js player in combination with require.js, you have to add this configuration to require.js.

```javascript

// require.js config
requirejs.config({
	// Other configuration
	shim: {
		// Other shims
		'https://playout.3qsdn.com/bin/hls.min.js': {deps: ['require'], exports: "sdnMSE"}
	}
});

// later in code
window.sdnMSE = sdnMSE;
```
Back to [index](../README.md).