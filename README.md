# semi
smaller semantic

http://github.com/doabit/semantic-ui-sass

you need only
http://github.com/doabit/semantic-ui-sass/tree/master/app/assets/stylesheets

and work with prepros.io as normal.

edit font, etc.

load smalles css semnatic 1.
Ideally semnatic 1 loads after pg images
and then after all, load semantic 2


On page where you need js or 'rare':
http://jsdelivr.com/package/npm/semantic-ui?path=dist%2Fcomponents


ex:

loadjs([ '//cdn.jsdelivr.net/npm/semantic-ui@2.3.1/dist/components/sidebar.min.js'


loadjs.ready(['style'], function () { //load large css
	loadjs([ '/assets/css/semnatic2.css'
	], 'css2', {
		async: false //required due to loadjs bug with bundles
	})
})


separate, icons used by setup:
- http://ionicons.com/usage