dfs_8queens(current_state, row=0):
    
if row == 8:  # All queens placed
        return current_state
    
    for col in range(8):  # Try all columns in order
        if is_valid(current_state, row, col):
            new_state = current_state + (col,)
            result = dfs_8queens(new_state, row + 1)
            if result is not None:
                return result
    return None  # Backtrackdef dfs_8queens(current_state, row=0):
    
