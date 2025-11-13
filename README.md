# aztec_repo

Aztec is a privacy-first zkEVM rollup that brings programmable privacy and scalability to Ethereum using zero-knowledge proofs, enabling private transactions and hybrid public/private workflows
def save_log_entry(entry: dict) -> None:
    log = load_log()
    log.append(entry)
    with LOG_PATH.open("w", encoding="utf-8") as f:
        json.dump(log, f, ensure_ascii=False, indent=2)
