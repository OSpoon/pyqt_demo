##### 1.安装 PyQt5
##### 2.安装 PyQt5-tools
##### 3.-m PyQt5.uic.pyuic  $FileName$ -o $FileNameWithoutExtension$.py
##### 4.run.py

    from PyQt5 import QtWidgets
    from main import Ui_Dialog


    if __name__=="__main__":
        import sys
        app=QtWidgets.QApplication(sys.argv)
        widget=QtWidgets.QDialog()
        ui=Ui_Dialog()
        ui.setupUi(widget)
        widget.show()
        sys.exit(app.exec_())