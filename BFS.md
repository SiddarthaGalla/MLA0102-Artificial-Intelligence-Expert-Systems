BREADTH FIRST SEARCH

CREATE empty set Visited
CREATE empty Queue Q

ENQUEUE StartNode into Q
ADD StartNode to Visited

WHILE Q is not empty DO
    Node ← DEQUEUE from Q
    VISIT Node
    FOR each Neighbor of Node in Graph DO
        IF Neighbor not in Visited THEN
            ADD Neighbor to Visited
            ENQUEUE Neighbor into Q
        END IF
    END FOR
END WHILE
