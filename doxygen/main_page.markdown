# This title gets eaten by Doxygen

# DOT graph {#section_dot}

@dot
digraph graphname {
  a [ label="Main page" ];
  b [ label="DOT graph" URL="@ref section_dot" ];
  c [ label="MSC sequence diagram" URL="@ref section_msc" ];
  d [ label="PlantUML diagram" URL="@ref section_plantuml" ];
  e [ label="Dia diagram" URL="@ref section_dia" ];
  f [ label="Images" URL="@ref section_images" ];
  a -> b;
  a -> c;
  a -> d;
  a -> e;
  a -> f;
}
@enddot

# MSC sequence diagram {#section_msc}

@msc
a [label="Client", URL="@ref section_client"],b [label="Server", URL="@ref section_server"];
a=>b [label="SYN"];
b=>a [label="SYN-ACK"];
a=>b [label="ACK"];
@endmsc

# PlantUML diagram {#section_plantuml}

@startuml
Client -> Server: SYN
Server -> Client: SYN-ACK
Client -> Server: ACK
@enduml

# Dia diagram {#section_dia}

@diafile internet.dia "Dia diagram" width=6cm

# Images {#section_images}

@image html people.svg
@image latex people.eps "People image" width=\textwidth

# Reference targets {#section_reference_targets}

## Client description {#section_client}

## Server description {#section_server}

