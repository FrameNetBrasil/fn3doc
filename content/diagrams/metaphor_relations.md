# http://www.graphviz.org/content/cluster

digraph G {
  graph [fontname = "Handlee"];
  node [fontname = "Handlee"];
  edge [fontname = "Handlee"];
  rankdir=LR;

    
  Metaphor1 [shape=square color=blue fontcolor=blue]
  Metaphor2 [shape=square color=blue fontcolor=blue]
  
  isSourceSubCaseOfMetaphor [shape=diamond]
  isTargetSubCaseOfMetaphor [shape=diamond]
  isSourceAndTargetSubCaseOfMetaphor [shape=diamond]
  isRelatedToMetaphor [shape=diamond]
  isRelatedToMetaphorBySource [shape=diamond]
  isRelatedToMetaphorByTarget [shape=diamond]
  isEntailedByMetaphor [shape=diamond]
  makesUseOfMetaphor [shape=diamond]
  hasTransitiveSubpart1Metaphor [shape=diamond]
  hasTransitiveSubpart2Metaphor [shape=diamond]
  isADualMetaphor [shape=diamond]
  isAMappingWithingMetaphor [shape=diamond]
  
  Metaphor1 -> isSourceSubCaseOfMetaphor -> Metaphor2
  Metaphor1 -> isTargetSubCaseOfMetaphor -> Metaphor2
  Metaphor1 -> isSourceAndTargetSubCaseOfMetaphor -> Metaphor2
  Metaphor1 -> isRelatedToMetaphor -> Metaphor2
  Metaphor1 -> isRelatedToMetaphorBySource -> Metaphor2
  Metaphor1 -> isRelatedToMetaphorByTarget -> Metaphor2
  Metaphor1 -> isEntailedByMetaphor -> Metaphor2
  Metaphor1 -> makesUseOfMetaphor -> Metaphor2
  Metaphor1 -> hasTransitiveSubpart1Metaphor -> Metaphor2
  Metaphor1 -> hasTransitiveSubpart2Metaphor -> Metaphor2
  Metaphor1 -> isADualMetaphor -> Metaphor2
  Metaphor1 -> isAMappingWithingMetaphor -> Metaphor2
  
  
}
