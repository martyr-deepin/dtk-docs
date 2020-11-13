# Prueba en Español


```cpp
#include "TetrisMainWindow.h"
#include <DApplication>
#include <DWidgetUtil>

DWIDGET_USE_NAMESPACE

int main(int argc, char *argv[])
{
    DApplication terisApp(argc, argv);
    // Set application base attribute and infomation
    terisApp.setAttribute(Qt::AA_UseHighDpiPixmaps);
    terisApp.setOrganizationName("LinuxDeepin");
    terisApp.setApplicationName("DeepinTetris");

    // set main window of tetris
    TetrisMainWindow tetrisMainWindow;
    tetrisMainWindow.setMinimumSize(1024, 768);
    tetrisMainWindow.setWindowFlags(Qt::WindowCloseButtonHint);
    tetrisMainWindow.show();
    moveToCenter(&tetrisMainWindow);
    return terisApp.exec();
}
```