The `datadog_logs` sink was not re-constructing ddtags that may have been parsed upstream by the `datadog_agent` source's `parse_ddtags` setting. The sink log encoding was fixed to re-assemble the tags into a unified string that the Datadog logs intake expects.