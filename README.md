
#  Architecture


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
```