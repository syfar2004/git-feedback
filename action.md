    # add a sample output
    outputs:
      example: ${{ steps.print-something.outputs.example }}
    steps:
      - name: Print something
        id: print-something
        run: echo "example=Hello World" >> $GITHUB_OUTPUT