cocos2d-x-notes
===============

Node 
---------------
遍历子节点方式

    for (auto& child : node->getChildren())
    {
        if (child)
        {
            Widget* widgetChild = dynamic_cast<Widget*>(child);
            if (widgetChild)
            {
                log(widgetChild->getName());
            }
        }
    }
