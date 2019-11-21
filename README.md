# python-srt2ass
Python script to convert Subtitle formats from `.srt` to `.ass`. Forked from [ewwink/python-srt2ass](https://github.com/ewwink/python-srt2ass) to change line ending to CRLF (as SubStation Alpha format spec states that ssa scripts are DOS text files) and apply my own preferred style.

## Requirements ##

* [Python 2.7](https://www.python.org/downloads/) (recommend)
* Windows/Linux/Mac/Android

## How to use ##

```python srt2ass.py "file"```

## Sample ##
using command line

    python srt2ass.py file1.srt
    
or

    python srt2ass.py file1.srt file2.srt file3.srt

using as module

    from srt2ass import srt2ass
    
    assSub = srt2ass("file.srt")
    print 'ASS subtitle saved as: ' + assSub
    # ASS subtitle saved as: file.ass


