# JSDOMInit
JS DOM init

```JS
 jQuery(() => {
	
    const __content = function( objectElem = {} ) { this.target = objectElem; }	
    
    __content.prototype.init = function() {
       
        let $__structure = this.target; 

        console.log($__structure);
    }	
        
   // init 
   const __app = function( oe ) { new __content( oe ).init(); }
    
   __app({ target  :  '.structure' });
    
 });



```

```JS
jQuery(() => {
	
 const NielsOfficeHover = function( objectElem = {} ) {
	
  this.target = objectElem;	 
	 
 }	
 
 NielsOfficeHover.prototype.init = function() {
	
  let objectData = this.target;
  let __dataID   = objectData.ID;
	 
  jQuery(__dataID).bind('mouseenter', function() {
	 
     alert('Your cursor getting enter within HTML Element! ');
      
  });	
	 
 }	
 	
 // init 
 const NielsOffice = function( oe ) {
	
  const Success = new NielsOfficeHover( oe );
	Success.init();
 }
 
 // USAGE:
 NielsOffice({
	
   ID    : '#dataID',
   Class : 'Class-a'
	 
 });
 
});
```

```JS

// check func exist
// Check if function exist jQuery 
function test() {
  console.log('Welcome to W3Docs');
}
//Call the function above if it exists.
if (typeof test === "function") {
  test();
}

// Check if function exist Vanilla 
function abc(){
}
!!window.abc; // return true
!!window.abcd; // return false

```
