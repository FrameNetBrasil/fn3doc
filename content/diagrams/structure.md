
digraph G {
  graph [fontname = "Handlee"];
  node [fontname = "Handlee"];
  edge [fontname = "Handlee"];
  rankdir=LR;

  bgcolor=transparent;

  Frame [shape=square color=blue fontcolor=blue]
  Bindings [shape=square color=blue fontcolor=blue]
  FrameFamily [shape=square color=blue fontcolor=blue]
  Inference [shape=square color=blue fontcolor=blue]
  Role [shape=square color=blue fontcolor=blue]
  LexicalUnit [shape=square color=blue fontcolor=blue]
  Metaphor [shape=square color=blue fontcolor=blue]
  Example [shape=square color=blue fontcolor=blue]
  Mapping [shape=square color=blue fontcolor=blue]
  MetaphorFamily [shape=square color=blue fontcolor=blue]
  Entailment [shape=square color=blue fontcolor=blue]
  
  hasBindings [shape=diamond]
  hasBoundRole1 [shape=diamond]
  hasBoundRole2 [shape=diamond]
  isInFrameFamily [shape=diamond]
  isFrameSubFamilyOf [shape=diamond]
  hasInference [shape=diamond]
  isInferenceOfFrame [shape=diamond]
  hasRoles [shape=diamond]
  hasLexicalUnit [shape=diamond]
  hasExample [shape=diamond]
  hasMappings [shape=diamond]
  hasSourceRole [shape=diamond]
  hasTargetRole [shape=diamond]
  hasEntailment [shape=diamond]
  hasEntailedMetaphor [shape=diamond]
  hasSourceInference [shape=diamond]
  hasTargetInference [shape=diamond]
  hasSourceFrame [shape=diamond]
  hasTargetFrame [shape=diamond]
  isInMetaphorFamily [shape=diamond]
  isMetaphorSubFamilyOf [shape=diamond]
  
  Frame -> hasBindings -> Bindings
  Bindings -> hasBoundRole1 -> Frame
  Bindings -> hasBoundRole2 -> Frame
  Frame -> isInFrameFamily -> FrameFamily
  FrameFamily -> isFrameSubFamilyOf -> FrameFamily
  Frame -> hasInference -> Inference
  Inference -> isInferenceOfFrame -> Frame
  Frame -> hasRoles -> Role
  Frame -> hasLexicalUnit -> LexicalUnit
  Metaphor -> hasExample -> Example
  Metaphor -> hasMappings -> Mapping
  Mapping -> hasSourceRole -> Role
  Mapping -> hasTargetRole -> Role
  Metaphor -> hasEntailment -> Entailment
  Entailment -> hasEntailedMetaphor -> Metaphor
  Entailment -> hasSourceInference -> Inference
  Entailment -> hasTargetInference -> Inference
  Metaphor -> hasSourceFrame -> Frame
  Metaphor -> hasTargetFrame -> Frame
  Metaphor -> isInMetaphorFamily -> MetaphorFamily
  MetaphorFamily -> isMetaphorSubFamilyOf -> MetaphorFamily
  
}