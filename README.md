# Elixir Key-Value Store

This project is a key-value (KV) store written in Elixir, demonstrating a simple and efficient way to manage key-value pairs. The architecture includes a registry and bucket system for organizing and retrieving data.

# Architecture

        # Registry -> PID(0.100.0)
        {
            %{ # Names
                "shopping" => PID(0.200.0)
            },
            %{  # Refs
                REF1234: "shopping"
            }
        }

        # Bucket -> PID(0.200.0)
        # Ref -> 1234
        %{
            "milk" => 1,
            "eggs" => 2
        }
