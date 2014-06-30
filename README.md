google-code-export
==================

Export your Google Code project to XML.

    git clone git://github.com/mconf/google-code-export.git
    easy_install BeautifulSoup
    cd google-code-export/src

Standard parsing:

    python main.py -p myproject -s 1 -c 100

Filtering by label (only saves issues with this label):

    python main.py -p myproject -s 1 -c 100 -l "Component-MyComponentName"

Specify a classic Netscape cookies.txt file in order to get full user information, instead of the masked usernames:

    python main.py -p myproject -s 1 -c 100 -j cookies.txt

Also look at `src/users.dat` and `src/status.dat` for users and statuses
mappings.
