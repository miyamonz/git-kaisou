parent repo に対して、subdirという名前のgit repoを入れる場合

すでにsubdirがgit repoの時に`git add subdir` とすると、submoduleとして認識される

それ以外
- subdirのファイルをparentでcommitしたあと、subdirでgit init
- subdirのファイルをparentでcommit

などは、submoduleとならずに、互いに独立してリポジトリとして動く。
subdir内でcommitしても、parentから見たらまだchanged fileやuntrackedfileとなる

parentで出力したdstやbinなどを時系列管理したい時には入れ子構造は使えるかも
