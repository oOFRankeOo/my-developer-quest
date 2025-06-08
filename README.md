def fibonacci(n: int) -> list[int]:
    """Trả về dãy Fibonacci dài n số (n ≥ 1)."""
    if n <= 0:
        raise ValueError("n phải ≥ 1")
    seq = [0, 1]
    while len(seq) < n:
        seq.append(seq[-1] + seq[-2])
    return seq[:n]

if __name__ == "__main__":
    so_phan_tu = 10
    print(f"Dãy Fibonacci ({so_phan_tu} số đầu tiên): 
