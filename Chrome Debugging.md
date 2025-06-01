
1. Console Tab - first place to look for errors

2. Elements Tab - this is a depiction of the DOM. 
     - it represents the HTML as node tree where each node is a part of our HTML

     - notice the <script>. These aren't in our source index.html. We'll talk about it later 
       in this course.

     - <pm-root ng-version-14.0.3"> ...(</pm-root>) this is our selector tag and you will see the 
       HTML defined in our component template

3. Sources Tab 
     - there's a debugger option available 
     - For Angular Only 
        - since Angular CLI uses webpack, our typescript files are listed under 
          the webpack node. And because Anglar CLI serve features generates the map files, we can debug 
          our TypeScript code directly.

        - navigate to webpack:// --> src --> app --> app.component --> set a breakpont on "PageTitle
          and click refresh --> break will be hit

     - Debugger shortcuts: 
          F8 = resume script. 
          F9 = Step
          F10 = step over next function call
          F11 = step into next function call
          Shift + F11 = step out of current function

     - VS Code Short Cuts
         Use Ctrl+Shift+O to quickly jump to a header in the current file.
         Use Ctrl+T to search through headers across all Markdown files in the current workspace.

         Path Completions:
           Path completions help with create links to files and images. 
         These paths are shown automatically by IntelliSense as you type the 
         path of an image or link, and can also be manually requested by 
         using Ctrl+Space.

4. Network Tab
    - enable  "preserve log" 
    - enable "All"
    - disable "Cache"
    - when tracing http calls such as GET, do in Chrome:
        F8 --> Network --> select "Fetch/XHR --> look under "Column Name" 

    - under Column Name... you will see the object passed to the server. 
      Example "Tickets" or "Products"
      
    - Click "Tickets" and you will see the following:
    
    - link to: https://code.visualstudio.com/docs/languages/markdown
    
    - images in network tab 
        ![alt text](<Example of Network Tab in Chrome-1.jpg>)
        ![alt text](<Example of Rsponse Header Network Tab in Chrome-1.jpg>)
        ![alt text](<Example of PayLoad Network Tab in Chrome-1.jpg>)
        ![alt text](<Example of FormData Network Tab in Chrome-1.jpg>)


  - Method 1 - how to disable/enable the javascript in Chrome

        Open Chrome Dev Tool - F12 --> settings (Cog wheel) --> Preference
           --> scroll down to Debugger --> check/uncheck Disable Javascript


  - Method 2 - How to disable javascript in Chrome

        ctl + shift + p  (run command)

        Run Command panel appears
        
        start typing javascript

        select "Disable Javascript"

        hit enter to run the command -->