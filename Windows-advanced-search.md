# 🔍 **Windows Advanced Search Operators (File Explorer & Start Search)**

## ✅ **1. File Name & Text Search**

* `someword`          Search file names + file contents  
* `filename:report`   Search only in file names          
* `*keyword*`         Wildcard search                    
* `"exact phrase"`    Exact phrase                       

---

## ✅ **2. File Type Search**

* `ext:.pdf`        Files with .pdf extension  
* `kind:document`   All documents              
* `kind:picture`    Images                     
* `kind:video`      Videos                     
* `kind:music`      Music files                
* `kind:program`    EXE + apps                 
* `type:pdf`        PDF documents              

**Common file kinds:**

* `kind:folder`
* `kind:email`
* `kind:calendar`
* `kind:contacts`
* `kind:notes`

---

## ✅ **3. Date Filters**

* `datemodified:today`            Modified today             
* `datemodified:yesterday`        Modified yesterday         
* `datemodified:this week`        This week                  
* `datemodified:2024`             Any file modified in 2024  
* `datemodified:>1/1/2024`        Modified after this date   
* `datecreated:<2024-05-01`       Created before this date   
* `date:2024-01-01..2024-03-01`   Between two dates          

---

## ✅ **4. Size Filters**

* `size:tiny`        0–10 KB              
* `size:small`       10–100 KB            
* `size:medium`      100 KB–1 MB          
* `size:large`       1–16 MB              
* `size:huge`        16–128 MB            
* `size:gigantic`    128 MB+              
* `size:>500MB`      Larger than 500MB    
* `size:1MB..50MB`   Between 1 and 50 MB  

---

## ✅ **5. File Attributes**

* `attributes:readonly`   Only read-only files  
* `attributes:system`     System files          
* `attributes:hidden`     Hidden files          
* `attributes:archive`    Archive bit set       

Combine:

```
attributes:system hidden
```

---

## ✅ **6. Folder Location Filters**

* `folder:Downloads`   Only inside Downloads     
* `path:C:\Work`       Search only in this path  

---

## ✅ **7. Metadata Search (Very Powerful)**

Works for images, music, office files, etc.

### Images:

```
dimensions:1920x1080
camera:Canon
tag:vacation
orientation:landscape
```

### Music:

```
artist:eminem
album:revival
genre:rock
length:>3:00
```

### Documents:

```
author:John
title:"project plan"
```

---

## ✅ **8. Boolean Operators**

* `term1 AND term2`   Must contain both                
* `term1 OR term2`    Either term                      
* `term1 NOT term2`   Include term1 but exclude term2  
* `term1 -term2`      Same as NOT                      

Examples:

```
report AND 2024
logo NOT old
pdf OR docx
```

---

## ✅ **9. Combine Operators (Pro Level)**

### Example 1 — Find all PDFs modified this month:

```
kind:document ext:pdf datemodified:this month
```

### Example 2 — Photos larger than 5MB taken with Samsung:

```
kind:picture size:>5MB camera:Samsung
```

### Example 3 — All Excel files created between two dates:

```
ext:xlsx datecreated:2024-01-01..2024-05-31
```

### Example 4 — Search inside contents (force):

```
content:"invoice number"
```

---

## 💎 **Special Hidden Operators (Few People Know)**

* `store:`          Indexed locations                    
* `is:attachment`   Attached files in emails             
* `sharedwith:`     Who the file is shared with          
* `tag:`            Windows file tags                    
* `date:`           Smart date filter (all date fields)  

