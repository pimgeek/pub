## Test Dagre-D3

<input id="show_gosol" type="button" value="GoSol" onclick="switchDisplay('gosol_canvas');tryDraw();" />

<div id="gosol_canvas">
  <input id="hide_gosol" type="button" value="×" onclick="undoDisplay('gosol_canvas');" />
  <div>
    <div id="debugInfo"></div>
    <div id="output">
      <svg width=800 height=600>
        <g/>
      </svg>
    </div>
  </div>
</div>

<script id="dot_code" type="text/graphviz">
digraph {
  a -> b;
}
</script>

<script type="text/javascript" src="../leo/d3.min.js"></script>
<script type="text/javascript" src="../leo/graphlib-dot.js"></script>
<script type="text/javascript" src="../leo/dagre-d3.min.js"></script>
<script type="text/javascript" src="../leo/dagre_utils.js"></script>
<script type="text/javascript" src="../leo/gosol_node_actions.js"></script>