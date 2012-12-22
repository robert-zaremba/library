= H1 nowa strona

treść jest tutaj!!

    class X(object):
        def __init__(self, val=None):
            self._x = val
    
        def x1(self): # mamamama
            """Helper"""
            return self._x
    
        def x2(self,val):
            """Helper"""
            self._x = val
            return val
        x = property(x1,x2, lambda: 0, doc="""Helper doc""")
    
    x=X('aa')
    x.x='ab'
    print x.x
    print x.x.__doc__
    x.x.doc = 'hej'

koniec kodu
