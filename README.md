# Annotations in chinese of underscore.js
==============================

[underscore.js中文注释（带笔记）](http://iissnan.com/underscore/docs/underscore.html)

## 更新步骤

1.  添加`underscore.js`的源代码仓库作为上游仓库:

        git remote add upstream git://github.com/documentcloud/underscore.git
    
2.  在`master`分支上检出`upstream/master`上的`underscore.js`
    
        git checkout upstream/master -- underscore.js
    
3. 切换到`gh-pages`分支
    
        git checkout gh-pages
    
4. 在`gh-pages`上合并`master`分支的代码
    
        git merge master
    
5. 处理冲突（会有大量的冲突，源代码或者注释的部分）
        
        git add underscore.js

6. 冲突处理完成后，生成文档（需要安装[docco](http://jashkenas.github.com/docco/)）
    
        docco underscore.js
    
7. 提交，推送
