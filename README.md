# spark

CSVAddrWriter writer = new CSVAddrWriter(output_file);
		
		Files.lines(Paths.get(NCOAConstants.PATH + input_file)).map(s -> parseAddresLine(s)).forEach(address -> processRecord(address,guideFileDataset,writer));
