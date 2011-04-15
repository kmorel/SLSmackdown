project(SLSmackdown NONE)

cmake_minimum_required(VERSION 2.8)

include(UseLATEX.cmake)

set(images
  images/TransparentOutput.png
  images/OpaqueOutput.png
  images/AccumulativeCompositeOrder.pdf
  images/TreeCompositeOrder.pdf
  images/CompositeImprovements0256.pdf
  images/CompositeImprovements2048.pdf
  images/InterlaceDiagram.pdf
  images/Interlace.pdf
  images/InterlaceJumpshot.pdf
  images/TelescopeDiagram.pdf
  images/TelescopeCompositeIntrepidSMP.pdf
  images/TelescopeCompositeIntrepidSMPZoomed.pdf
  images/TelescopeCompositeIntrepidVN.pdf
  images/PartitionCollectIntrepidFull.pdf
  images/CollectRounds.pdf
  images/PartitionCollectIntrepidReduced.pdf
  images/ScalingTransparent.pdf
  images/ScalingOpaque.pdf
  images/ScalingCollectTransparent.pdf
  images/ScalingCollectOpaque.pdf
  )

add_latex_document(SLSmackdown.tex
  BIBFILES SLSmackdown.bib
  IMAGES ${images}
  )
