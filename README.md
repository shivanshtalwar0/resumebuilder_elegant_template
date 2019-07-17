# resume_builder
![sample image](https://github.com/shivanshtalwar0/resumebuilder_elegant_template/raw/master/Screen%20Shot%202019-07-17%20at%2010.17.18%20PM.png)
> My stupendous Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

```
# update data
to update your data go to data() in index.vue file in pages directory to change resume data.   
# find data() in index.vue 
``` 
data(){  
return{  
myname:"Your xyz name",  
myimage:"/myprofile.png"  
//Remember to put your profile image in static folder  
experience:[....], //replace with your own data  
educations:[...],//replace with your own data  
.  
.  
.  
.  
so on after saving file it will be updated instantly in browser too   
}  
}  
```
For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).
