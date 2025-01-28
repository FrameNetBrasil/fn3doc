digraph G {
  graph [fontname = "Handlee"];
  node [fontname = "Handlee"];
  edge [fontname = "Handlee"];
  rankdir=LR;

    
  Frame1 [shape=square color=blue fontcolor=blue]
  Frame2 [shape=square color=blue fontcolor=blue]
  
  isSubcaseOfFrame [shape=diamond]
  makesUseOdFrame [shape=diamond]
  incorporateFrameAsRole [shape=diamond]
  isSubprocessOfFrame [shape=diamond]
  isInAScalarOppositionToFrame [shape=diamond]
  isInCausalRelationToFrame [shape=diamond]
  isAPerspectiveOnFrame [shape=diamond]
  isRelatedToFrame [shape=diamond]
  
  Frame1 -> isSubcaseOfFrame -> Frame2
  Frame1 -> makesUseOdFrame -> Frame2
  Frame1 -> incorporateFrameAsRole -> Frame2
  Frame1 -> isSubprocessOfFrame -> Frame2
  Frame1 -> isInAScalarOppositionToFrame -> Frame2
  Frame1 -> isInCausalRelationToFrame -> Frame2
  Frame1 -> isAPerspectiveOnFrame -> Frame2
  Frame1 -> isRelatedToFrame -> Frame2
  
  
}
