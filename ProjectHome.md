text flow is a trivial generator of RFC like ASCII call flow (sequence diagrams) written in Clojure.

The easiest way to run is from the Clojure REPL, as follow:

```
(flow [Alice Bob Tzach]
 [[mmm Tzach Bob]
 [xxx Bob Alice]
 []
 [zzz Alice Tzach]])
```

Which will give you the following pure ASCII result:

```
Alice                Bob                Tzach
 |                   |         mmm       |
 |                   |<------------------|
 |         xxx       |                   |
 |<------------------|                   |
 |                   |                   |
 |         zzz       |                   |
 |-------------------------------------->|
```


Visit the online version here:
http://textflowonline.appspot.com/