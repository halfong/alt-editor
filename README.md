alt-editor
==========

a wysiwyg content editor base on html5 contenteditable &amp; js range object



<h1>Usage</h1>

<a href='http://rangy.googlecode.com/svn/trunk/currentrelease/rangy-core.js'>rangy</a>
<a href='http://egofang.com/lib/client/egofn.js'>egofn.js</a>
And the <b>alteditor.js.</b>


if u need to transfer element<b>#zone<b> into an alt-editor.
<code>
  var k = new alteditor(document.getElementById('zone'),{
      //here is all the options for normal use
      inline:["strong","small","del"],  // tagName of elements avalible in editor(style them to style text style)
			spoor:"F",  //placeholder when toggle tags
			// uploader:null,  under coding
			// maxImgWidth:540,
			// maxImgHeight:540,
			save:function(){	//ctrl+s will trigger save function
				console.log("save hasn't customed");return false;
			},
			lineBreaker:function(){ //node to insert when break line
				return document.createElement('br');
			},
  });
</code>



<h1>Broswer Support</h1>
Not test right now.
