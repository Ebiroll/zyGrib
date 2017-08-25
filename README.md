# zyGrib

To compile on Centos

yum install jasper-devel
yum install bzip2-devel
yum install libnova-devel


QT4-5 stuff

	treeWidget->header()->setResizeMode (QHeaderView::ResizeToContents);


replace,

table->verticalHeader()->setResizeMode(QHeaderView::ResizeToContents);  
table->horizontalHeader()->setResizeMode(QHeaderView::ResizeToContents); 

with the following Qt 5 code:

table->verticalHeader()->setSectionResizeMode(QHeaderView::ResizeToContents); 
table->horizontalHeader()->setSectionResizeMode(QHeaderView::ResizeToContents); 

http://doc.qt.io/qt-5/qheaderview.html#setSectionResizeMode