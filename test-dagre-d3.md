## Test Dagre-D3

<link rel="stylesheet" type="text/css" href="../leo/gosol_node_styles.css" />
<link rel="stylesheet" type="text/css" href="../leo/dagre.css" />

<input id="show_gosol" type="button" value="GoSol" onclick="doDisplay('dot_code');tryDraw();" />

<div id="gosol_canvas">
  <svg width="800" height="600">
    <g></g>
  </svg>
</div>

<textarea id="dot_code" type="text/graphviz">
digraph FlyingLogic {
  rankdir=LR;
  eid1 [label="A" style="filled" fillcolor="white"];
  eid8 [label="E" style="filled" fillcolor="white"];
  gid1 [labelType="html" label="<div style='padding: 10px;' onclick='top.editGraph(\"digraph FlyingLogic { rankdir=LR; eid1 [label=A ]; eid8 [label=E ]; subgraph cluster_eid13 { label=UnFolded eid2 [label=B ]; eid4 [label=C ]; eid5 [label=1 shape=circle ]; eid10 [label=OR shape=circle]; eid14 [label=D ]; } eid1 -> eid5; eid5 -> eid2; eid5 -> eid4; eid4 -> eid10; eid10 -> eid8; eid2 -> eid14; eid14 -> eid10; } \");tryDraw();'>Folded</div>" style="fill: silver;"]
  eid1 -> gid1;
  gid1 -> eid8;
}
</textarea>

<script type="text/javascript" src="../leo/d3.min.js"></script>
<script type="text/javascript" src="../leo/graphlib-dot.js"></script>
<script type="text/javascript" src="../leo/dagre-d3.min.js"></script>
<script type="text/javascript" src="../leo/dagre_utils.js"></script>
<script type="text/javascript" src="../leo/gosol_node_actions.js"></script>
