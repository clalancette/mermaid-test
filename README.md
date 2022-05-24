
```mermaid
gantt
    title ROS 2 Release process
    dateFormat  YYYY-MM-DD
    section Before previous release
    Find ROS Boss    :a1, 2022-03-08, 28d
    Discourse naming thread     :a2, after a1  , 21d
    Collate names from Discourse thread :after a2, 1d
    section Another
    Task in sec      :2022-01-12  , 12d
    another task      : 24d
    
    click a1 href "https://www.google.com.com"
```

<body>
  <div class="mermaid">
    gantt
      dateFormat  YYYY-MM-DD

      section Clickable
      Visit mermaidjs           :active, cl1, 2014-01-07, 3d
      Print arguments         :cl2, after cl1, 3d
      Print task              :cl3, after cl2, 3d

      click cl1 href "https://mermaidjs.github.io/"
      click cl2 call printArguments("test1", "test2", test3)
      click cl3 call printTask()
  </div>

  <script>
    var printArguments = function(arg1, arg2, arg3) {
      alert('printArguments called with arguments: ' + arg1 + ', ' + arg2 + ', ' + arg3);
    }
    var printTask = function(taskId) {
      alert('taskId: ' + taskId);
    }
    var config = {
      startOnLoad:true,
      securityLevel:'loose',
    };
    mermaid.initialize(config);
  </script>
</body>
