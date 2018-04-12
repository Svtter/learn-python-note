Notifier
=========


OSX
----


.. code:: python


    import os

    # The notifier function
    def notify(title, subtitle, message):
        t = '-title {!r}'.format(title)
        s = '-subtitle {!r}'.format(subtitle)
        m = '-message {!r}'.format(message)
        os.system('terminal-notifier {}'.format(' '.join([m, t, s])))

    # Calling the function
    notify(title    = 'A Real Notification',
           subtitle = 'with python',
           message  = 'Hello, this is me, notifying you!')

refer
^^^^^
https://stackoverflow.com/questions/17651017/python-post-osx-notificatio://stackoverflow.com/questions/17651017/python-post-osx-notification

