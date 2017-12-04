# plasma-profile
A uml profile project for Plasma. UML profiles based on Eclipse Papyrus
must be edited with Papyrus itself and this repo 
is dedicated solely to the maintenance of the Plasma 
profile.

Edited profiles must be "defined" using Papyrus 
and saved, then coped to a specific version, found in the
root directory of the repo. 

Defined versions of the profile are then copied to the plasma-eclipse plugins
repo and the Plasma repo.

Note that each "definition" of the profile creates an additional eclipse content
section as below. All but the topmost/newest one needs to be manually
removed. :)
 
<eAnnotations>
<content>...</content>  
<content>...remove me...</content>  
</eAnnotations>

In fact the more time the profile is saved the more <content>...</content> sections
are not only added by Papyrus links them together. So when one section is removed
invalid references can occur. 

The best approach seems to be removing all the Eclipse specific annotations entirely from
the profile including diagrams unfortunately, then saving/registering it, resulting
in one single valid <content> section. 

