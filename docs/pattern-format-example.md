v0.0.1 (2024-03-19)

# ZenPattern Format Example

## Basic Single Pattern

ZenPattern-1.0
type: single
id: BASIC001

meta:
  name: Simple Dot Pattern
  author: zenito
  created: 2024-03-19
  version: 1
  tags: [minimal, dots]

compat:
  min_app: 1.0
  features: [basic]

patterns:
  - id: DOT8080
    name: basic_dot
    type: base
    props:
      weight: normal
      style: dotted
      spacing: 2

## Pattern Family

ZenPattern-1.0
type: family
id: SHAPES001

meta:
  name: Basic Geometric Family
  author: zenito
  created: 2024-03-19
  version: 1
  tags: [geometric, minimal, basic]

compat:
  min_app: 1.0
  features: [basic, animation]

patterns:
  - id: SOLID8080
    name: solid_base
    type: base
    props:
      weight: normal
      style: solid
  
  - id: DOT88080
    name: dotted_variant
    type: variant
    base: SOLID8080
    props:
      style: dotted
      spacing: 2
  
  - id: DASH8080
    name: dashed_variant
    type: variant
    base: SOLID8080
    props:
      style: dashed
      dash_length: 4
      spacing: 2

extensions:
  custom_props:
    animation_support: true
    rtl_support: true

## Pattern Collection

ZenPattern-1.0
type: collection
id: STATUS001

meta:
  name: Status Indicators
  author: zenito
  created: 2024-03-19
  version: 1
  tags: [status, indicators]

compat:
  min_app: 1.0
  features: [basic, status]

patterns:
  - id: READY001
    name: ready_indicator
    type: base
    props:
      style: solid
      weight: bold
  
  - id: PROC001
    name: processing
    type: base
    props:
      style: dotted
      animation: pulse
  
  - id: WAIT001
    name: waiting
    type: base
    props:
      style: dashed
      dash_pattern: [2,2]

extensions:
  custom_props:
    status_colors: false
    animation_enabled: true 